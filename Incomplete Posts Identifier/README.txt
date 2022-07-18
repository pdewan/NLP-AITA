Step 1 & 2: Feature Engineering & Data Splitting
1. download "Step 1 _ 2_ Feature Engineering + Data Splitting.ipynb" from NLP-AITA -> Incomplete Posts Identifier -> Code.
2. download "Incomplete Posts Identifier.xlsx" from NLP-AITA -> Incomplete Posts Identifier -> Data.
3. Convert "Incomplete Posts Identifier.xlsx" to "COMP All courses.csv" by combining all sub-sheets in "Incomplete Posts Identifier.xlsx" into a single sheet and converting it to a CSV file. Alternatively,  you can split the courses into several CSV files according to their names and semesters.
4. move "COMP All courses.csv" to the same folder as "Step 1 _ 2_ Feature Engineering + Data Splitting.ipynb".
5. open "Step 1 _ 2_ Feature Engineering + Data Splitting.ipynb" using Anaconda3, Jupyter Notebook.
6. Regardless of your choice about how to arrange the data, after the feature engineering step, the output file will be two CSV files, one for the training data and the other for the test data. The output files will be in the same folder as your IPYNB and original CSV files.
* Note that you will get an error in the cell right after "Reason feature 4" since the IBM API was used in the code and the API keys together with the API service URL are omitted. To make the code work, you need to get your own API keys and the API service URL. Consult Dr. Dewan for how to get the API keys and the API service URL.

Step 3: Neural Network
1. download "Step 3_ Neural Network.ipynb" from NLP-AITA -> Incomplete Posts Identifier -> Code.
2. open "Step 3_ Neural Network.ipynb" using Anaconda3, Jupyter Notebook.
3. In the second cell, change the variable "file" to the CSV files you got in "Step 1 & 2: Feature Engineering & Data Splitting". Do not add the "(train)" or "(test)" suffix as the program will find the corresponding files automatically. Change the variable "embedding_model" to the one you want to use. The supported "embedding_model" is shown in the second cell. Change the variable "neural_network" to the one you want to use. The supported "neural_network" is shown in the second cell.
4. Once you set the file, embedding model, and neural network, the training will begin automatically. After the training finishes, a ".h5" file will be generated and be in the same folder as your IPYNB and original CSV files. The ".h5" file is the trained model. You may use it on the testing data set.