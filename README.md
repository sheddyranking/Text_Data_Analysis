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

#### Negative comment Visuation.
![Negative_comment](https://user-images.githubusercontent.com/42388234/156906533-eddf03ea-0648-4b6e-b168-9d0bce3216f8.Png)

#### Positive comment Visuation.
![Positive_comment](https://user-images.githubusercontent.com/42388234/156906543-c7927959-686c-41a6-ab99-8fa01958497f.Png)



### Problem Statement  => Emoji  Analysis.

-- `!pip install emoji` on `Jupyter notebook`.

-- `pip install emoji` on `conda prompt` or `Cmd prompt` open and run as `administrator`

#### Note:
After iterating the `emoji_list`, you need to compute it into `frequncies`, which means you need to come up with data in the form of `Dict`. this can be implemented completely from `Scratch`, or using `count`. But in this analysis we shall be using `Collections models`. 

#### Emoji Visualization.
![emoji](https://user-images.githubusercontent.com/42388234/157077250-cb57d5ca-deda-400c-8879-597563990c14.png)


### Problem Statement  => Collecting the Entire data of Youtube.

-- The first way to do this by using the `OS`, interating with the `OS` and using a `path` to access all the files.

-- The second way is `Glob`, which is consider to be the best way.

#### Most Common econdings for reading data.

-- `latin`, `UTF-8`, `iso-8859-1` (essential in reading complex data example is japanese data), `cp-1252`


### Problem Statement  => Which Category has the Maximum Likes.

The category file was clean and coverted to `dict`, then,the `Category_name` in the `dict` was map with `category_id` in the `full_df` and store in a `column` created in the `full_df`.

-- finding the maximum likes in the category can be archived with `groupby` as well but we used `boxplot` to visualized. 

#### Visualized most liked category.
![most_like_category](https://user-images.githubusercontent.com/42388234/157568635-4981313b-6991-4523-89ae-22fdd3893993.Png)


### Problem Statement  =>  Find out weather Audience are Engaged or not.

The three most important `keys` to consider when solving this kind of problem are `Like_rate`, `Dislike-rate`, `Comment_rate`.

#### Like rate:
![likes_rate](https://user-images.githubusercontent.com/42388234/157765781-39171b0f-dfbd-421c-99b1-7f99bc10e215.png)


#### Analysis weather your Viewes will affect your likes or not.
In this case you can use `Scatter plot` or `Regplot` to check and also `correlation` and visualized it using `heatmap`

##### Note.
when using `seaborn regplot` in `jupyter notebook` always set `ci=None`, for it to execute.


### Problem Statement  => Analyse trending videos

In this project the data frame had only `channel_tile` and `video_id`, so we used a `groupby` function to group the `video_id's` according to there `channel_title`. and renamed the `video_id's` column to `total_video` according to there `channel_title` respectfully, the channel with the highest count of `video_id` had the trending vidoes. 

### Problem Statement  => Does Punctuation in a title and tags have any relations with views,likes,dislikes and comments?.

We have to extracts all the `punctuations` from `title`, `channel_title` or `tags`, and this can be done completely from `scratch` or using python build in modules like `Regular expression`, `Strings`. in this project we shall use the `string` module. 

--- To check if the punctuatons will affect the `views`,`likes`,`dislikes` or `comments`. use `correlatoin` check the `count punctuations` on the `views`,`likes`,`dislikes` or `comments`. 








