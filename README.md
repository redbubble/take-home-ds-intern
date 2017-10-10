# Redbubble Take-home data science test

## Context
We often need to get a representative sample of searches for different purposes.
For instance, to test our search engine, or to evaluate the quality of our results.

A representative sample is a set of queries that contains _many_ very popular queries, _some_ common queries, and _a few_ of the less popular queries.

## Task
Write a program that creates a *representative sample* based on a list of queries.

The program should take two arguments: the input file with the list of all queries,
 and the number of queries to return in the sample. It should write the query
 sample in a file output.txt.

 You are welcome to use the programming language you feel the most comfortable with.


**Sample input** (queries.csv)
```
Query,Frequency
Shakespeare,733
Falstaff,471
Richard III (Duke of Gloucester),409
Henry V,377
```
The Frequency columns count how many time that search was made over the last 30 days.
The higher the number, the more popular the query.

**Sample execution**
```bash
# Generate a representative sample of 3 queries from queries.csv
query_sampler queries.csv 3
```

**Sample output** (output.txt)
```
Shakespeare
Shakespeare
Henry V
```
Note that queries may be repeated in the output.


## Resources
[Sample query file](./queries.csv) (adapted from [OS Shakespeare](https://www.opensourceshakespeare.org/views/plays/characters/chardisplay.php))
