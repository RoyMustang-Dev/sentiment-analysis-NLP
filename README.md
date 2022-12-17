# ${\color{white}Sentiment\ Analysis: NLP}$

***Note:*** ` This Project is an end-to-end implimentation, of Sentiment Analysis using various NLP techniques, for an Orgainization. So dataset information is not available for Public usage, anyone attempting to impliment this can use their own datasets!!! `

## Software And Tools Requirements

1. [GithubAccount](https://github.com)
2. [HerokuAccount](https://heroku.com)
3. [VSCodeIDE](https://code.visualstudio.com/)
4. [GitCLI](https://git-scm.com/downloads)
5. [AnacondaPackage/JupyterNoteBook](https://www.anaconda.com/products/distribution)

## Creata a New Environment and Activate!!

```
conda create -p venv python==3.9 -y
conda activate venv/
```

## Install all the Required Libraries!!

```
pip install -r requirements.txt
```
# Getting started with the Project!!

## ${\color{cyan}1.\ Problem \ Statement:}$
### ${\color{darkgray}To\ analyze\ the\ Sentiments\ of\ the\ Learners\ who\ are\ posting\ thier\ queries\ in\ QnA\ Forums\ of\ an\ organization}$
&nbsp;

## ${\color{cyan}2.\ Dataset \ Info:}$
### ${\color{darkgray}The\ dataset\ is\ not\ available,\ however\ the\ information\ pertaining\ to\ the\ columns\ used\ are\ given\ below,}$ ${\color{darkgray}so\ that\ anyone\ can\ make\ their\ own\ dataset\ and\ impliment\ this\ project.}$
&nbsp; 
*  ${\color{darkgray}ID:\ the\ unique\ identifier\ used\ to\ map\ the\ learners\ who\ posted\ their\ queries.}$
*  ${\color{darkgray}Content:\ a\ descriptive\ paragraph\ written\ by\ learners\ in\ order\ to\ explain\ their\ query.\ We\ will\ analyze\ this\ column.}$
*  ${\color{darkgray}Happiness\ Rating:\ the\ ratings\ given\ by\ the\ learners.}$

&nbsp;

## ${\color{cyan}3.\ NLTK\ Approach:}$
### ${\color{darkgray}Since\ we\ already\ have\ a\ dataset,\ we'll\ approach\ the\ problem\ with\ the\ following\ machine\ learning\ modelling\ framework.}$
&nbsp;
*  ${\color{darkgray}Step1:\ Cleaning and EDA.}$
*  ${\color{darkgray}Step2:\ Pre-processing\ and\ Feature\ Engineering.}$
*  ${\color{darkgray}Step3:\ Applying\ NLTK\ Life\ Cycle\ which\ involves\ below\ mentioned\ steps-}$ <br/> 
&nbsp; ` a. Tokenize-> Word Tokenizer`<br/> 
&nbsp; ` b. Removing Punctuations-> String Punctuations`<br/>
&nbsp; ` c. Removing Stopwords`<br/>
&nbsp; ` d. Position Tags`<br/>
&nbsp; ` e. Wordnet PosTags`<br/>
&nbsp; ` f. Lemmatize-> Word Lemmatizer`<br/>
&nbsp; ` g. Sentiment Analysis-> TextBlobs' Polarity`<br/>
&nbsp; ` h. Converting the above generated Sentiment Scores into String(Positive,Negative,Neutral) and Making new Column`<br/>
&nbsp; ` i. Sentiment Driven EDA`<br/>
&nbsp; ` j. Term Frequency Analysis`<br/>
&nbsp;

## ${\color{cyan}4.\ Topic\ Modeling:}$
### ${\color{darkgray}Since\ we\ already\ have\ Sentiment\ Scores\ and\ we've\ done\ Sentiment\ driven\ EDA.}$ 
### ${\color{darkgray} We\ will\ start\ with\ Topic\ Modeling.\ There\ are\ various\ ways\ but\ we\ are\ using\ the\ following\ methodologies.}$
&nbsp;
*  ${\color{darkgray}Count Vectorizer}$
*  ${\color{darkgray}Latent\ Dirichlet\ Allocation (LDA)\ Topic\ Modeling,\ also\ using\ "pyLDAvis"\ which\ is\ LDA\ visualization\ python\ library}$
*  ${\color{darkgray}Non-Negative\ Matrix\ Factorization (NMF),\ with\ TF-IDF (Term\ Frequency—Inverse\ Document\ Frequency)\ method}$
&nbsp;

### ${\color{darkgray}When\ we\ are\ finished\ with\ Topic\ Modeling,\ we\ will\ also\ do\ a\ topic\ model\ driven\ EDA}$

&nbsp;

## ${\color{cyan}5.\ Batch\ Processing:}$
### ${\color{darkgray}This\ step\ is\ not\ mandatory,\ I\ am\ only\ doing\ this\ to\ get\ a\ clearer\ picture\ and\ also\ because}$ 
### ${\color{darkgray}the\ dataset\ is\ comparatively\ huge\ and\ Performing\ Topic\ Modeling\ on\ such\ a\ huge\ dataset}$ 
### ${\color{darkgray}needs\ the\ ample\ amount\ of\ Computing\ Resources\ and\ time.}$