baadalvm@master:~/hadoop/hadoop-1.2.1/bin$ ./hadoop fs -mkdir /A4/grade_folder_1
Warning: $HADOOP_HOME is deprecated.

WARNING: An illegal reflective access operation has occurred
WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/home/baadalvm/hadoop/hadoop-1.2.1/hadoop-core-1.2.1.jar) to method sun.security.krb5.Config.getInstance()
WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
WARNING: All illegal access operations will be denied in a future release
baadalvm@master:~/hadoop/hadoop-1.2.1/bin$ ./hadoop fs -ls /A4/
Warning: $HADOOP_HOME is deprecated.

WARNING: An illegal reflective access operation has occurred
WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/home/baadalvm/hadoop/hadoop-1.2.1/hadoop-core-1.2.1.jar) to method sun.security.krb5.Config.getInstance()
WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
WARNING: All illegal access operations will be denied in a future release
Found 1 items
drwxr-xr-x   - baadalvm supergroup          0 2019-11-14 02:24 /A4/grade_folder_1








baadalvm@master:~/hadoop/hadoop-1.2.1/bin$ ./hadoop fs -put ~/Grades/student_records.csv  A4/grades_folder_1
Warning: $HADOOP_HOME is deprecated.

WARNING: An illegal reflective access operation has occurred
WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/home/baadalvm/hadoop/hadoop-1.2.1/hadoop-core-1.2.1.jar) to method sun.security.krb5.Config.getInstance()
WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
WARNING: All illegal access operations will be denied in a future release
baadalvm@master:~/hadoop/hadoop-1.2.1/bin$ ./hadoop jar ~/Grades/grades.jar AverageGrade /user/baadalvm/A4/grades_folder_1 /user/baadalvm/A4/grades_folder_out_1

