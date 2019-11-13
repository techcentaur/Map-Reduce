baadalvm@master:~/hadoop/hadoop-1.2.1/bin$ ./hadoop jar ~/Word_classes/wordcount.jar WordCount /user/baadalvm/A4/input_words2 /user/baadalvm/A4/output_new_folder_2
Warning: $HADOOP_HOME is deprecated.

WARNING: An illegal reflective access operation has occurred
WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/home/baadalvm/hadoop/hadoop-1.2.1/hadoop-core-1.2.1.jar) to method sun.security.krb5.Config.getInstance()
WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
WARNING: All illegal access operations will be denied in a future release
19/11/14 02:15:29 WARN mapred.JobClient: Use GenericOptionsParser for parsing the arguments. Applications should implement Tool for the same.
19/11/14 02:15:30 INFO input.FileInputFormat: Total input paths to process : 1
19/11/14 02:15:30 INFO util.NativeCodeLoader: Loaded the native-hadoop library
19/11/14 02:15:30 WARN snappy.LoadSnappy: Snappy native library not loaded
19/11/14 02:15:30 INFO mapred.JobClient: Running job: job_201911131834_0004
19/11/14 02:15:31 INFO mapred.JobClient:  map 0% reduce 0%
19/11/14 02:15:42 INFO mapred.JobClient:  map 27% reduce 0%
19/11/14 02:15:43 INFO mapred.JobClient:  map 31% reduce 0%
19/11/14 02:15:44 INFO mapred.JobClient:  map 35% reduce 0%
19/11/14 02:15:45 INFO mapred.JobClient:  map 41% reduce 0%
19/11/14 02:15:46 INFO mapred.JobClient:  map 44% reduce 0%
19/11/14 02:15:48 INFO mapred.JobClient:  map 50% reduce 0%
19/11/14 02:15:49 INFO mapred.JobClient:  map 53% reduce 0%
19/11/14 02:15:52 INFO mapred.JobClient:  map 56% reduce 8%
19/11/14 02:15:55 INFO mapred.JobClient:  map 60% reduce 8%
19/11/14 02:15:58 INFO mapred.JobClient:  map 63% reduce 8%
19/11/14 02:16:01 INFO mapred.JobClient:  map 67% reduce 8%
19/11/14 02:16:04 INFO mapred.JobClient:  map 69% reduce 8%
19/11/14 02:16:20 INFO mapred.JobClient: Task Id : attempt_201911131834_0004_m_000001_0, Status : FAILED
java.io.IOException: Could not obtain block: blk_8893582323320857235_1079 file=/user/baadalvm/A4/input_words2
	at org.apache.hadoop.hdfs.DFSClient$DFSInputStream.chooseDataNode(DFSClient.java:2460)
	at org.apache.hadoop.hdfs.DFSClient$DFSInputStream.blockSeekTo(DFSClient.java:2252)
	at org.apache.hadoop.hdfs.DFSClient$DFSInputStream.read(DFSClient.java:2415)
	at java.base/java.io.DataInputStream.read(DataInputStream.java:100)
	at org.apache.hadoop.util.LineReader.readDefaultLine(LineReader.java:205)
	at org.apache.hadoop.util.LineReader.readLine(LineReader.java:169)
	at org.apache.hadoop.mapreduce.lib.input.LineRecordReader.nextKeyValue(LineRecordReader.java:139)
	at org.apache.hadoop.mapred.MapTask$NewTrackingRecordReader.nextKeyValue(MapTask.java:531)
	at org.apache.hadoop.mapreduce.MapContext.nextKeyValue(MapContext.java:67)
	at org.apache.hadoop.mapreduce.Mapper.run(Mapper.java:144)
	at org.apache.hadoop.mapred.MapTask.runNewMapper(MapTask.java:764)
	at org.apache.hadoop.mapred.MapTask.run(MapTask.java:364)
	at org.apache.hadoop.mapred.Child$4.run(Child.java:255)
	at java.base/java.security.AccessController.doPrivileged(Native Method)
	at java.base/javax.security.auth.Subject.doAs(Subject.java:423)
	at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1190)
	at org.apache.hadoop.mapred.Child.main(Child.java:249)

attempt_201911131834_0004_m_000001_0: WARNING: An illegal reflective access operation has occurred
attempt_201911131834_0004_m_000001_0: WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/home/baadalvm/hadoop/hadoop-1.2.1/hadoop-core-1.2.1.jar) to method sun.security.krb5.Config.getInstance()
attempt_201911131834_0004_m_000001_0: WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
attempt_201911131834_0004_m_000001_0: WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
attempt_201911131834_0004_m_000001_0: WARNING: All illegal access operations will be denied in a future release
19/11/14 02:16:21 INFO mapred.JobClient:  map 44% reduce 8%
19/11/14 02:18:07 INFO mapred.JobClient:  map 51% reduce 8%
19/11/14 02:18:10 INFO mapred.JobClient:  map 54% reduce 8%
19/11/14 02:18:13 INFO mapred.JobClient:  map 58% reduce 8%
19/11/14 02:18:16 INFO mapred.JobClient:  map 62% reduce 8%
19/11/14 02:18:19 INFO mapred.JobClient:  map 66% reduce 8%
19/11/14 02:18:22 INFO mapred.JobClient:  map 69% reduce 8%
19/11/14 02:18:27 INFO mapred.JobClient:  map 72% reduce 8%
19/11/14 02:18:30 INFO mapred.JobClient:  map 76% reduce 8%
19/11/14 02:18:33 INFO mapred.JobClient:  map 80% reduce 16%
19/11/14 02:18:36 INFO mapred.JobClient:  map 87% reduce 16%
19/11/14 02:18:38 INFO mapred.JobClient:  map 89% reduce 16%
19/11/14 02:18:39 INFO mapred.JobClient:  map 94% reduce 16%
19/11/14 02:18:42 INFO mapred.JobClient:  map 97% reduce 16%
19/11/14 02:18:44 INFO mapred.JobClient:  map 100% reduce 16%
19/11/14 02:18:49 INFO mapred.JobClient:  map 100% reduce 100%
19/11/14 02:18:50 INFO mapred.JobClient: Job complete: job_201911131834_0004
19/11/14 02:18:50 INFO mapred.JobClient: Counters: 30
19/11/14 02:18:50 INFO mapred.JobClient:   Map-Reduce Framework
19/11/14 02:18:50 INFO mapred.JobClient:     Spilled Records=1066072
19/11/14 02:18:50 INFO mapred.JobClient:     Map output materialized bytes=259176
19/11/14 02:18:50 INFO mapred.JobClient:     Reduce input records=19776
19/11/14 02:18:50 INFO mapred.JobClient:     Virtual memory (bytes) snapshot=10362146816
19/11/14 02:18:50 INFO mapred.JobClient:     Map input records=30000000
19/11/14 02:18:50 INFO mapred.JobClient:     SPLIT_RAW_BYTES=452
19/11/14 02:18:50 INFO mapred.JobClient:     Map output bytes=333359430
19/11/14 02:18:50 INFO mapred.JobClient:     Reduce shuffle bytes=259176
19/11/14 02:18:50 INFO mapred.JobClient:     Physical memory (bytes) snapshot=949686272
19/11/14 02:18:50 INFO mapred.JobClient:     Reduce input groups=4944
19/11/14 02:18:50 INFO mapred.JobClient:     Combine output records=602252
19/11/14 02:18:50 INFO mapred.JobClient:     Reduce output records=4944
19/11/14 02:18:50 INFO mapred.JobClient:     Map output records=30030181
19/11/14 02:18:50 INFO mapred.JobClient:     Combine input records=30612657
19/11/14 02:18:50 INFO mapred.JobClient:     CPU time spent (ms)=104140
19/11/14 02:18:50 INFO mapred.JobClient:     Total committed heap usage (bytes)=580911104
19/11/14 02:18:50 INFO mapred.JobClient:   File Input Format Counters 
19/11/14 02:18:50 INFO mapred.JobClient:     Bytes Read=213250994
19/11/14 02:18:50 INFO mapred.JobClient:   FileSystemCounters
19/11/14 02:18:50 INFO mapred.JobClient:     HDFS_BYTES_READ=213251446
19/11/14 02:18:50 INFO mapred.JobClient:     FILE_BYTES_WRITTEN=14261531
19/11/14 02:18:50 INFO mapred.JobClient:     FILE_BYTES_READ=13711782
19/11/14 02:18:50 INFO mapred.JobClient:     HDFS_BYTES_WRITTEN=59849
19/11/14 02:18:50 INFO mapred.JobClient:   Job Counters 
19/11/14 02:18:50 INFO mapred.JobClient:     Launched map tasks=8
19/11/14 02:18:50 INFO mapred.JobClient:     Launched reduce tasks=1
19/11/14 02:18:50 INFO mapred.JobClient:     SLOTS_MILLIS_REDUCES=184052
19/11/14 02:18:50 INFO mapred.JobClient:     Total time spent by all reduces waiting after reserving slots (ms)=0
19/11/14 02:18:50 INFO mapred.JobClient:     SLOTS_MILLIS_MAPS=154798
19/11/14 02:18:50 INFO mapred.JobClient:     Total time spent by all maps waiting after reserving slots (ms)=0
19/11/14 02:18:50 INFO mapred.JobClient:     Rack-local map tasks=3
19/11/14 02:18:50 INFO mapred.JobClient:     Data-local map tasks=5
19/11/14 02:18:50 INFO mapred.JobClient:   File Output Format Counters 
19/11/14 02:18:50 INFO mapred.JobClient:     Bytes Written=59849

