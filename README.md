# Text_Data_Analysis
This is a Text Data Analysis Project Involving `(YouTube Case Study)`.

### Problem Statement  => Sentiment Analysis.

 ### Package1:
 There are many Sentiment Packages such as `Vader`, `Pacy`. In this project i am using `TextBlob` which is a `NLP` library. 
 
When considering ` Texblob Sentiment Analysis`, there are two keys involved which are `Polarity` and `Subjectivity`.
 
 -- `Polarity`:  Which ranges from  `[-1 to +1]` for negative and positive sentiments.
 
 -- `Subjectivity`: When there are no `Sentiments` in a sentence. 
 
 ### Error_Handling
 Use `try`,`except` to handle error in your code.
 
### Package2:
The second package I'll be using to perform `visualization` on the  sentiment Analysis is `Wordcloud`.

   -- `wordcloud`:analysis give regard to the `keyword` with the bigger `Font`, therfore any `keyword` with this attribute has the `higher priority`.
   
   -- `wordcloud` : data must also be stored in `String` nature before being passed.
   
#### Instaling wordcloud.
`wordcloud` can be tricky when installing . irrespective of command prompt or conda prompt.. open and run as `administrator` and excute the following line of codes below.

-- for conda.
`conda install -c https://conda.anaconda.org/conda-forge wordcloud` 

-- For command prompt.
```
git clone https://github.com/amueller/word_cloud.git
cd word_cloud
pip install .

```

#### stopword. 
This are words that donot make any sense in Analysis. such as `He`, `Him`, `Is`, `The`. 

-- `wordcloud` has parameters that removes this stopwords . ie `(stopwords = reset(STOPWORDS)`.


### Problem Statement  => Emoji  Analysis.

-- `!pip install emoji` on `Jupyter notebook`.
-- `pip install emoji` on `conda prompt` or `Cmd prompt` open and run as `administrator`

#### Note:
After iterating the `emoji_list`, you need to compute it into `frequncies`, which means you need to come up with data in the form of `Dict`. this can be implemented completely from `Scratch`, or using `count`. But in this analysis we shall be using `Collections models`. 



