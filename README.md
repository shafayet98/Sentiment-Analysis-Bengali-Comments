Sentiment-Analysis-Bengali-Comments
# Sentiment Analysis on Bengali Youtube Drama Comments (NLP)
In this particular project the goal was to detect the positive and negative sentiment of Bengali Youtube Drama Comments. In order to acheieve the goal, a Natural Langage Processing (NLP) system was designed that was trained using Bangla Youtube Comments in order to distinguish between the sentiments.<br />
The positive sentiment refers to compliments of the drama or actors, wherease the negative sentiment refers to hate speech, negative comments, bullying the actors etc. 

### Systematic steps were taken for designing a proper classifier:<br/>
1. Data Collection using Youtube Data API
2. Basic preprocessing on the data
3. Labelling the dataset
4. Merging labeled data with existing labeled dataset
5. Final preprocessing
6. Feature Extraction
7. Fitting into the model

### Short description of each files are given below:
1. **youtube_bangla_data_collection:**  Collects comments using youtube data api
2. **youtube_data_preprocess:** <br/>
    a) Remove  HTML Tag, <br/>
    b) Remove Punctuation and <br/>
    c) Remove Double Space <br/>
3. **Labelling the comments**
4. **Preprocess_version_01:** <br/> 
    a) drop the unlabelled comments <br/>
    b) separate the positive and negative comments <br/>
5. **Preprocess_version_02:** <br/> 
    a) Merge the labeled data with the existing dataset <br/>
    b) separate the positive and negative example. <br/>
6. **Preprocess_version_03:** <br/>
    a) Line stripping, <br/>
    b) remove punctation <br/>
    c) remove english words <br/>

### Feature extraction Techniques:
1. Count Vectorisation
2. Frequency based Feature Extraction
3. TF-IDF

### Basic preprocessing for all the feature extraction techniques:
1. Removing stop words
2. Stemming
3. Tokenization

### Models:
1. Logistic Regression
2. Multinomial Naive Bayes
3. Gaussian Naive Bayes 
4. Support Vector Machine
5. Random forest classifier

### Dataset:
1. generated using Youtube Data API(Unlabelled): youtube_comment.csv
2. generated using Youtube Data API(Labelled): youtube_comment.xlsx
3. Final Merged Dataset: final_shuffled_dataset.csv

*There was two dataset that was merged in order to create a balance dataset.*
1. [BN-Dataset](https://github.com/sazzadcsedu/BN-Dataset)
2. Youtube Data API generated dataset.
Eventually both datasets were merged to create the final dataset. 

**The combined dataset contains 11,908 positive samples and 4,892 negative samples. The SVM model obtaind highest accuracy of 85.09%.**




