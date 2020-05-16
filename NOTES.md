### 2016.04.09
1. [Deploying Shiny apps with shinyapps.io](http://www.r-bloggers.com/deploying-shiny-apps-with-shinyapps-io/)

### 2016.07.04
1. [Different Approaches to Unknown Words in a
Hidden Markov Model Part-of-Speech Tagger](http://stp.lingfil.uu.se/~nivre/statmet/haulrich.pdf).

### 2016.04.05
1. Transition Matrix needs revision based on [this](https://lagunita.stanford.edu/c4x/Engineering/CS-224N/asset/slp4.pdf).


### 2016.04.02

1. [The markovchain Package: A  Package for Easily Handling Discrete Markov Chains in R, page 5](https://cran.r-project.org/web/packages/markovchain/vignettes/an_introduction_to_markovchain_package.pdf)
2. [all.equal may be a better operator to compare objects](http://stackoverflow.com/questions/9508518/why-are-these-numbers-not-equal)

### 2016.03.31
Week 4 very useful materials:

1. [Implementing n-grams for next word prediction with tau package](http://stackoverflow.com/questions/31316274/implementing-n-grams-for-next-word-prediction)
2. [tau Package](https://cran.r-project.org/web/packages/tau/tau.pdf).
3. [Natural Language Processing: A Model to Predict a Sequence of Words](http://www.modsimworld.org/papers/2015/Natural_Language_Processing.pdf) - Very detailed paper
4. [http://www.dormantroot.com/2015/02/predicting-words-using-n-gram-modeling.html](http://www.dormantroot.com/2015/02/predicting-words-using-n-gram-modeling.html).
	* [https://github.com/dormantroot/Data-Science/blob/master/Capstone%20Project/PredictWord/predictNextWord.R](https://github.com/dormantroot/Data-Science/blob/master/Capstone%20Project/PredictWord/predictNextWord.R)

### 2016.03.27
1. [Very good explanation on back off by Coursera class mate](https://www.coursera.org/learn/data-science-project/module/VNKmf/discussions/V40gAPE3EeWFuw7QEATDpw)
2. Look into **Kneser-Ney Smoothing**

### 2016.03.26
1. [How to go parallel in R](http://www.r-bloggers.com/how-to-go-parallel-in-r-basics-tips/).

### 2016.03.25
1. [R: Increase heap size for rJava](http://www.bramschoenmakers.nl/en/node/726)

### 2016.03.24
1. [Natural Language Processing](https://rpubs.com/lmullen/nlp-chapter)

### 2016.03.23

1. [Guide to the N Gram Package](https://cran.r-project.org/web/packages/ngram/vignettes/ngram-guide.pdf)
2. [Package 'ngram'](https://cran.r-project.org/web/packages/ngram/ngram.pdf)
3. [Predictive Modeling with R and the caret Package](https://www.r-project.org/nosvn/conferences/useR-2013/Tutorials/kuhn/user_caret_2up.pdf)
4. Worth the read, potentially student's work. [http://rstudio-pubs-static.s3.amazonaws.com/39014_76f8487a8fb84ed7849e96846847c295.html](http://rstudio-pubs-static.s3.amazonaws.com/39014_76f8487a8fb84ed7849e96846847c295.html).
5. [Ray Jones response](https://www.coursera.org/learn/data-science-project/discussions/q_INCeZ_EeWohBKTpGZ3Aw/replies/GDGSMefKEeWPKQpBKpg03Q).
6. [Next word prediction benchmark](https://github.com/hfoffani/dsci-benchmark).

### 2016.03.19
1. [ISO 639-2 Language Codes](https://www.loc.gov/standards/iso639-2/php/code_list.php)
2. The function `tm_map` may have issue with "Snowballc' package - Resolution is to install it manually with `install.packages`. Refer [here](https://support.rstudio.com/hc/en-us/community/posts/200652293-Snowball-Stemmer-is-not-working-in-R-Studio).
3. [Sample code for transformation](http://stackoverflow.com/questions/25330753/more-efficient-means-of-creating-a-corpus-and-dtm). The sequence of transformation would affect the end results, say `stemDocument` comes before `removePunctuation`
4. [Stemming](https://en.wikipedia.org/wiki/Word_stem) removes affixes from words(E.g "run", "runs", "running" become "run")
5. [Text Mining The Complete Works of William Shakespeare](http://www.r-bloggers.com/text-mining-the-complete-works-of-william-shakespeare/).
6. [Stop Words](http://nlp.stanford.edu/IR-book/html/htmledition/dropping-common-terms-stop-words-1.html) are extremely common words that has little value in text mining activity.
7. `TermDocumentMatrix` can be transposed into `DocumentTermMatrix`. Each convenience depends on the number of documents and terms in the data.
8. [Basic Text Mining in R](https://rstudio-pubs-static.s3.amazonaws.com/31867_8236987cf0a8444e962ccd2aec46d9c3.html); Very good reference too.

### 2016.03.15

1. Create a generic function that performs data reduction.
	* Read file via `readLines`
	* Within for-loop; If `decide` is true then accumulate else skip
	* Very bad performance
2. How to read large text file efficiently ?
	* CLT - Sample only 1% data
	* Take note of special character "SUB" - Read file as binary
	* Make assumption that only the body texts are important - Corpus object hold a number of text documents
	* [https://www.youtube.com/watch?v=s3kKlUBa3b0](https://www.youtube.com/watch?v=s3kKlUBa3b0) from [https://www.coursera.org/learn/data-science-project/module/OkCmA/discussions/q_INCeZ_EeWohBKTpGZ3Aw](https://www.coursera.org/learn/data-science-project/module/OkCmA/discussions/q_INCeZ_EeWohBKTpGZ3Aw)
	* [R example for sampling](https://www.coursera.org/learn/data-science-project/module/mb9DN/discussions/CgJEA-nTEeWfwAohgaM63Q)
	* [Introduction to the "tm" Package](https://cran.r-project.org/web/packages/tm/vignettes/tm.pdf)
3. What is n-gram?
	* [https://www.coursera.org/learn/data-science-project/module/mb9DN/discussions/aFSPjunbEeWcTQpIg9bO1w](https://www.coursera.org/learn/data-science-project/module/mb9DN/discussions/aFSPjunbEeWcTQpIg9bO1w)
	* E.g. A single word is unigram, a pair is 2-gram
4. Markov Chain
	* [A very good reference](http://setosa.io/ev/markov-chains/)

### 2016.03.11

1. [faster for() loops in R](http://www.r-bloggers.com/faster-for-loops-in-r/)
	* It is **MUCH** faster to create the results an empty vector of the correct size.
	* R seems to be slow in allocating memory for objects.
2. [Speed up the loop operation in R](http://stackoverflow.com/questions/2908822/speed-up-the-loop-operation-in-r)
	* The power of vectorization.
	* Use vectorized commands, e.g. `ifelse` or `diff` is faster than the `apply` family. 

### 2016.03.10

1. [Text Mining Infrastructure in R](https://www.jstatsoft.org/article/view/v025i05)
  	* Consist of R Source Package and example.
2. [https://cran.r-project.org/web/views/NaturalLanguageProcessing.html](https://cran.r-project.org/web/views/NaturalLanguageProcessing.html)
  	* Worth exploring but not immediately useful. 