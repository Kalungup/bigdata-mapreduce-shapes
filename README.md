# bigdata-mapreduce-shapes

# Hadoop MapReduce – Shape Frequency Counter
### Hadoop Streaming MapReduce to count shapes (Big Data assignment)
This project runs a Hadoop Streaming MapReduce job to count the frequency of shapes in a dataset of 100,000 records.

## Files

- `mapper.py` – reads shapes (one per line) and emits `<shape> 1`
- `reducer.py` – sums counts per shape and outputs `<shape> total_count`
- `shapes_result.txt` – final frequencies from the Hadoop job

## Technologies

- Hadoop HDFS
- Hadoop Streaming
- Python (mapper & reducer)
- Linux shell / Zeppelin

## Final Output (100,000 shapes)

- circle: 6,973  
- diamond: 10,153  
- pentagon: 25,145  
- square: 12,966  
- star: 4,963  
- triangle: 39,800

This totals to 100,000, indicating that our Map-reducers are working correctly
