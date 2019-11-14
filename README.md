So this repository will contain:
- How to run a program for map-reduce on hadoop
- I will also shut down 2 datanodes will running, and see the result of it in map-reduce process

I may miss something, drop an issue if you don't understand something. Or if there is some mistake, or you point out a grammatical mistake, feel free to point it out or drop a pull request.


## Map-Reduce

Let's stop all processes and format the namenode, if there are any still going on from my previous assignments
- ./stop-all.sh 
- ./hadoop namenode -format

If secondarynamenode is not getting started, listen on the netstat and see if there is an address already in binding.
- netstat --listen

Start the namenode and datanodes of hadoop / running JPS will show that a data or namenode is running on that machine
- ./start-all.sh 
- jps

Now, we run hadoop binary with a jar + from a filepath + with Class name + with location of input data as a filepath of hadoop file-system + path of the output as a filepath of hadoop file-system (+ breaks the arugments) 
- ./hadoop jar ~/Word_classes/wordcount.jar WordCount /user/baadalvm/A4/input_words /user/baadalvm/A4/output_word11
Make a directory in Hadoop FS (I'm gonna say it HFS from now)
- ./hadoop fs -mkdir A4/input_word2
List the contents for confirmation that it worked
- ./hadoop fs -ls A4/
```
WARNINGs: <IGNORE THE WARNINGS>
drwxr-xr-x   - baadalvm supergroup          0 2019-11-14 02:24 /A4/input_word2
```
Put the data in the HFS to use
- ./hadoop fs -put ~/input_data/bulk_names.txt  A4/input_words2
List the content of A4 folder in HFS
- ./hadoop fs -ls A4/










baadalvm@master:~/hadoop/hadoop-1.2.1/bin$ ./hadoop fs -put ~/Grades/student_records.csv  A4/grades_folder_1
Warning: $HADOOP_HOME is deprecated.

WARNING: An illegal reflective access operation has occurred
WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/home/baadalvm/hadoop/hadoop-1.2.1/hadoop-core-1.2.1.jar) to method sun.security.krb5.Config.getInstance()
WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
WARNING: All illegal access operations will be denied in a future release
baadalvm@master:~/hadoop/hadoop-1.2.1/bin$ ./hadoop jar ~/Grades/grades.jar AverageGrade /user/baadalvm/A4/grades_folder_1 /user/baadalvm/A4/grades_folder_out_1




