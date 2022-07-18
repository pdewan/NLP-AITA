Step 1: Data Cleaning
1. download "Step 1_ Data Cleaning.ipynb" from NLP-AITA -> Duplicate Posts Identifier -> Code.
2. download "train.csv" and "test.csv" from NLP-AITA -> Duplicate Posts Identifier -> Data.
3. move "train.csv" and "test.csv" to the same folder as "Step 1_ Data Cleaning.ipynb".
4. open "Step 1_ Data Cleaning.ipynb" using Anaconda3, Jupyter Notebook.
5. In the third cell of "Step 1_ Data Cleaning.ipynb", change the boolean variables (eg. hyper_cleaning = True) in the "data_cleaning" function to indicate the type of data cleaning you want. A detailed explanation of the variables is shown in the thrid cell, above the function body.
6. Once you choose the data cleaning type, the output file will be two CSV files, one for the training data and the other for the test data, with the corresponding data cleaning type as suffix (eg. if you choose hyper_cleaning = True, there will be a "(hyper_cleaned)" in your output CSV filename for both the training and testing data). The output files will be in the same folder as your IPYNB and original CSV files.

Step 2: Feature Engineering
1. download "Step 2_ Feature Engineering.ipynb" from NLP-AITA -> Duplicate Posts Identifier -> Code.
2. open "Step 2_ Feature Engineering.ipynb" using Anaconda3, Jupyter Notebook.
3. In the second cell, change the variable "data_clean_type" to the data cleaning type you chose in Step 1: Data Cleaning. The supported "data_clean_type" is shown in the second cell.
4. Once you set the data cleaning type, features will be extracted from the data automatically. The output will be two CSV files with the name "train_with_features + data_clean_type + .csv" and 'test_with_features + data_clean_type + .csv', where the "data_clean_type" is the one set by you before running the feature enginnering code. The output files will be in the same folder as your IPYNB and original CSV files.

Step 3: Neural Network
1. download "Step 3_ Neural Network.ipynb" from NLP-AITA -> Duplicate Posts Identifier -> Code.
2. open "Step 3_ Neural Network.ipynb" using Anaconda3, Jupyter Notebook.
3. In the second cell, change the variable "data_clean_type" to the data cleaning type you chose in Step 1: Data Cleaning. The supported "data_clean_type" is shown in the second cell. Change the variable "embedding_model" to the one you want to use. The supported "embedding_model" is shown in the second cell. Change the variable "neural_network" to the one you want to use. The supported "neural_network" is shown in the second cell.
4. Once you set the data cleaning type, embedding model, and neural network, the training will begin automatically. After the training finishes, a ".h5" file will be generated and be in the same folder as your IPYNB and original CSV files. The ".h5" file is the trained model. You may use it on the testing data set.