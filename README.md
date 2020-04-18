# WordCount

WordCount example reads text files and counts how often words occur (hadoop)

## Testing

1. Download the sources.
2. Compile to a .jar file (I have already compiled the java file under name wordcount.jar)
3. You need to copy data from local to HDFS using these commands:
- `hadoop dfs -mkdir <hdfs-dir> //not required in hadoop 0.17.2 and later`
- `bin/hadoop dfs -copyFromLocal <local-dir> <hdfs-dir>`
4. Use the following command `hadoop jar wordcount.jar wordcount [-m <#maps>] [-r <#reducers>] <in-dir> <out-dir>`: 
