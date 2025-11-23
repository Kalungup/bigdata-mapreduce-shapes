# 🛠️ Hadoop Big Data Analytics

This project contains Hadoop MapReduce programs for text analytics, including:

- Word Count
- Word Standard Deviation
- Unique word extraction
- Frequency analysis

## 📂 Repository Structure
data/             → Input text files  
src/              → Source code for MapReduce jobs  
jar/              → Compiled JAR files  
output/           → Hadoop output directory (ignored from Git)

## 🚀 Run Hadoop Jobs

### 1️⃣ Upload data to HDFS
hadoop fs -mkdir -p /user/pascal/input
hadoop fs -put data/*.txt /user/pascal/input

### 2️⃣ Word Count
hadoop jar jar/WordCount.jar wordcount.WordCount /user/pascal/input /user/pascal/output_wc
hadoop fs -cat /user/pascal/output_wc/part-r-00000

### 3️⃣ Word Standard Deviation
hadoop jar jar/WordStandardDeviation.jar wordstandarddeviation.WordSD /user/pascal/input /user/pascal/output_sd
hadoop fs -cat /user/pascal/output_sd/part-r-00000

## 🧰 Tech Stack
- Hadoop 3.x
- HDFS
- Java MapReduce (or Python streaming)
- Linux / Ubuntu (DSV VM)

## 👤 Author
Pascal Kalungu  
Technical Project Manager | Data Engineering | Big Data | AI
