# mapReduceAverage
Calculate Average value in WordCount MapReduce on Hadoop

The famous example of Word Count that can be found here [here](https://hadoop.apache.org/docs/current/hadoop-mapreduce-client/hadoop-mapreduce-client-core/MapReduceTutorial.html#Example:_WordCount_v1.0)
Shows a simple MapReduce that sets counter of words.

Here I set an example that instead of counting the words, will print out the average value of word count.

In order to do so, we changed the original program:

- We separated between combiner and reducer (it was the same class used for both puposes)
- We created a new reducer that accumulates the Average value accross the iterations and eventually prints the final value
