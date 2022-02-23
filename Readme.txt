Enviorment Required
1. Numpy , Matplotlib
2. All the data sets are stored in the google drive. so file path mentioned leads you to  google drive folder. If you want to run a local file , you need to change the path.

3. To train the mlp models , I downloaded the dataset , then preprocessed it by dividing it by 255 , and then passed it to feature extraction function. the output matrix of feature extraction function is then fed to the mlp models.

4.  I have uploaded two numpy file, which stores the weight parameter of the trained  models

5. aug_weight.npy   file stroes the weight matrices of the model trained on augmented data set. Its shape is (1,4)
     you can access the weights stored by indexing it 
     w_1 = aug_weight[0,0]
    b_1 =  aug_weight[0,1]
   w_2 =  aug_weight[0,2]
   b_2 = aug_weight[0,3]
where w_1 and b_1 are weights and biases of 1st layer and w_2 and b_2 are weights and biases of 2nd layer

6. similarly we have attached unaug_weight.npy file .It stores the weights and biases of the mlp model trained on unaugmented dataset.  The method to access it is same as above.
 
7. I have uploaded  two .ipynb files . 
 8 .   image augmentation.ipynb has all image transformation functions along with feature extraction function

9. MLP.ipynb file contains feed forward and back propagation alogorithm , Mlp function trained on  augmented and original data

10 . To train  the MLP model using your own data, comment the code where i have imported data , and rename your dataset as xdata and ydata with dimension (50000,512) , (50000,1) and for augmented model, data dimension should be (100000,512) , (100000,10).

11. To test my model accuracy using your own test data , comment the code where i am importing test data , subtitute your dataset as xdata_test and  ytest_data . 


