Yeah so this will contain steps and the reason why I did it. I may miss something, drop an issue if you don't understand something. Or if there is some mistake, or you point out a grammatical mistake, feel free to point it out or drop a pull request.

## Map-Reduce

Let's stop all processes and format the namenode, if there are any still going on from my previous assignments
 1983  ./stop-all.sh 
 1984  ./hadoop namenode -format
If secondarynamenode is not getting started, listen on the netstat and see if there is an address already in binding.
 1985  netstat --listen
Start the namenode and datanodes of hadoop
 1986  ./start-all.sh 
 1987  jps
 1988  ls
Now we run Map-reduce
 1989  history | grep input_words
 1990  ./hadoop jar ~/Word_classes/wordcount.jar WordCount /user/baadalvm/A4/input_words /user/baadalvm/A4/output_word11
 1991  cd ..
 1992  cd bin/
 1993  ./hadoop fs -mkdir A4/input_word2
 1994  ./hadoop fs -ls
 1995  ./hadoop fs -put ~/input_data/bulk_names.txt  A4/input_words2
 1996  ./hadoop fs -ls A4/
 1997  ./hadoop jar ~/Word_classes/wordcount.jar WordCount /user/baadalvm/A4/input_words2 /user/baadalvm/A4/output_word12
 1998  history


