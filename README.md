au.id.cxd.Math
==============

A collection of experiments focusing on processing tabular data. 

> At the moment I'm not spending much time working in F# and have been working more in scala. I've been experimenting with other statistical methods in my own scala library, but much of this work is sheerly for my own learning. There are already many good open source libraries available for performing much of the processes defined in this and my other library. Hence the implementation in this library is not necessarily the most efficient implementation. However it is rather a learning excersize that captures some of the process of working with the algorithms and language. If you're interested in this library you might also be interested in some of the experimentation I've been playing around with in the scala project [scala-au.id.cxd.math](https://github.com/cxd/scala-au.id.cxd.math). Currently the source base is not frequently updated as I'm busy with study (working on completing studies in math) and work outside of this project, although I've got plenty of ideas of more algorithms I'd like to implement I think I'm more likely to be experimenting in the scala project than this one for the near term.

The core library focuses on providing supporting methods for summarising data sets in the following ways.

1. It defines standard data types for raw data.
* String - labels and categories expressed as strings.
* NumericOrdinal - numeric ordinal ranges
* Continuous - continuous real values
* Bool - boolean values

A data set is described as a set of attributes which consist of a column and data type pair and a set of data columns 
each containing samples for the types represented by that column.


2. It provides some simple methods for summarisation.
* Basic statistics for each columnn
- average, variance, standard deviation, min, max etc.
* histograms
* CDF curves
* gaussian distributions

3. It provides some simple methods for approximating values based on the current sample.
* Regression for single values.

4. It provides some tools to display the summary information.
* au.id.cxd.Math.UI provides a WPF application with partial functionality for graphing summaries of the data.
* Current tinkering is to change this structure to a web application which will provide equivalent functionality.

Among other things, there are also a number of experiments with the following types of problems.
* Supervised learning - implementations of a simple backpropogration network, and a decision tree.
* Text analysis - bigram and unigram models using a bayesian model.
* Optimisation problems - experiments with an implementation of the simplex algorithm and 
integer programming branch and bound methods. 

The main useful tool has been the math ui which has proven useful at work when taking data from load tests 
and using it to provide some insight into the distribution, and similarity between counters used
for profiling different aspects of the systems under test.




