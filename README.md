# DM2024-Lab1-Master

ISA5810 Lab 1 Notebook

# Student Information
    Name: 陳映璇
    Student ID: r12528053
    GitHub ID: weew2000

# Instructions
1. First: do the take home exercises in the DM2024-Lab1-Master. You may need to copy some cells from the Lab notebook to this notebook. This part is worth 20% of your grade.
    - file : [DM2024-Lab1-Master.ipynb](./DM2024-Lab1-Master.ipynb)
    - 
2. Second: follow the same process from the DM2024-Lab1-Master on the new dataset. You don't need to explain all details as we did (some minimal comments explaining your code are useful though). This part is worth 30% of your grade.
    - file : [DM2024-Lab1-HW.ipynb](./DM2024-Lab1-HW.ipynb)

3. Third: please attempt the following tasks on the new dataset. This part is worth 30% of your grade.
    - file : [DM2024-Lab1-HW_3.ipynb](./DM2024-Lab1-HW_3.ipynb)

    - Generate meaningful new data visualizations.  
       **Search : New Data Visualization**
    - Generate TF-IDF features from the tokens of each text. This will generating a document matrix, however, the weights will be computed differently (using the TF-IDF value of each word per document as opposed to the word frequency). 
        **Search : TF-IDF (Term Frequency-Inverse Document Frequeny)**

    - Implement a simple Naive Bayes classifier that automatically classifies the records into their categories. Use both the TF-IDF features and word frequency features to build two seperate classifiers. Note that for the TF-IDF features you might need to use other type of NB classifier different than the one in the Master Notebook. Comment on the differences. 

        **Search : Data classification !**
        

4. Fourth: In the lab, we applied each step really quickly just to illustrate how to work with your dataset. There are somethings that are not ideal or the most efficient/meaningful. Each dataset can be handled differently as well. What are those inefficent parts you noticed? How can you improve the Data preprocessing for these specific datasets? This part is worth 10% of your grade.

    The thing I noticed in the data preprocessing is the unnecessary use of one-hot encoding for labels. One-hot encoding is not always necessary and may lead to inefficiencies.

    - Memory Consumption: One-hot encoding increases the size of your dataset. For example, in a classification task with 100 classes, one-hot encoding would transform each label into a 100-element vector, consuming more memory than needed, especially for large datasets.

    - Not necessary : Some algorithms (e.g. Naive Bayes) can work directly with integer-encoded labels. Applying one-hot encoding unnecessarily adds complexity and slows down the processing without any performance gain. For example, in binary classification (eg. Nostalgic_Sentiment_Analysis_of_YouTube_Comments_Data dataset), labels can be represented as 0 and 1. Using the one-hot vector (e.g., [0, 1] or [1, 0]) is redundant and inefficient.

5. Fifth: It's hard for us to follow if your code is messy, so please tidy up your notebook and add minimal comments where needed. This part is worth 10% of your grade.


