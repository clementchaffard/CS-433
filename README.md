# CS-433



We investigate the effect of batch size on training dynamics using stochastic gradient descent on a simple CNN model. We were able to observe how smaller batch sizes training approaches were able to converge faster than larger ones. This put us on the track. If our training method using larger batch size wasn't able to produce good results was because it failed to travel far enough in a reasonable number of training epochs. We slowly increased the learning rate and found an optimal learning rate of 0.1. We were able to recover up to 75\% accuracy using full batch training proving to be competitive against small batch size training method. The large batch size training method could prove to be very useful on more complex datasets where smaller batch size approaches fail to converge.



The code used for this project can be found in the code folder. The CNN used is coded in the models file, the MNIST data can be loaded using a fonction coded in the Load_data file, the functions used to train the model and compute it's accuracy are contained in the Train file. Finaly, all the results used in this project can be obtained by running the Main file. The number of trials was initialy set to 10 to obtain more consistent results. It can be reduced to 1 (variable n_trials) to improve running time.
