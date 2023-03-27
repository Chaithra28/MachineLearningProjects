Prerequisite: 
1. Latest python version installed on the system.
2. Conda Navigator through which Jupyter can be accessed.
3. You should have the training and test data sets from miner.
Follow the steps given below to execute the code:
1. Unzip the file and open the .ipynb file on Jupyter notebook.
2. Run the cells one by one till you see the step where the X_train, y_train, X_valid, y_valid are defined which looks as follows:
    X_train = train_data.Review.astype(str)
    y_train = train_data.label.astype(str)

    X_valid = valid_data.Review.astype(str)
    y_valid = valid_data.label.astype(str)
3. Skip the gridsearch cv as the step is used to find the best parameters and may take a long time to execute.
4. Run rest of the cells to fit the model and find accuracy.
5. The last step will save the test prediction file. Make change to the file name as per your requirement. Upload the test prediction file on miner to check the accuracy.