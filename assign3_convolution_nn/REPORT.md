        TASK 1: CLONE THIS REPO AND USE THIS PROJECT AS STARTER CODE[OPTIONAL]
        
        TASK 2: CONFIGURE[OPTIONAL] DATALOADER ACCORDING TO YOUR NEED OR USE YOUR OWN
        
        TASK 3: TRY TO TWEAK THE MODEL[OPTIONAL] TO FIT YOUR NEED OR DESIGN YOUR OWN MODEL OR USE PRETRAINED MODEL
                TIPS : RIGHT NOW MODEL IS IMPLEMENTED FOR 1 CLASS PROBLEM
        
        TASK 4: [OPTIONAL]IN TRAINER YOU NEED TO UPDATE YOUR LOSS FUNCTION
                TIPS : CHANGE IT TO FIT ON MULTICLASS CLASSIFICATION
                OR DESIGN YOUR OWN TRAINER
                
        TASK 5: [OPTIONAL]IN TRAINER YOU NEED TO UPDATE TRAINING LOOP,
                TIPS : YOU NEED TO CHANGE HOW ACCURACY IS CALCULATED
                OR DESIGN YOUR OWN TRAINER
        
        TASK 6: [OPTIONAL] IN TRAINER YOU NEED TO UPDATE TESTING LOOP, 
                TIPS : YOU NEED TO CHANGE HOW ACCURACY IS CALCULATED
                OR DESIGN YOUR OWN TRAINER
        
        TASK 7: RUN THE EXPERIMENT ON MINIMUM 10 CLASSES 
        
        TASK 8: CREATE A REPO OF YOUR PROJECT
        
        TASK 9: IN YOU REPORT SUBMIT FOLLOWING
                
                - LINK TO YOUR GITHUB REPO
                
                - BRIEF DETAILS OF ARCHITECTURE YOU USE
                        NOTE YOU CAN USE PRETRAINED ARCHITECTURE AS WELL
                
                - REPORTS OF EXPERIMENT RESULTS
                    ACCURACY 
                    GRAPHS OF LOSSES AND ACCURACY
                
                - REPORT FOLLOWING __ THAT YOU HAVE USED IN YOUR EXPERIMENT
                    - LOSS FUNCTION
                    - LEARNING RATE
                        -By reducing the learning rate by a factor of 10 (.0001 to .00001), the accuracy was somewhat improved. 
                        When the learning was .0001, the run yielded results with an average of just over 42%. After changing 
                        the learning rate to .00001, the average accuracy rose to just over 53%. 
                        -When increasing the learning rate, the average accuracy became considerably worse. Going from a learning
                         rate of .0001 to .0005 resulted in a decrease in average accuracy from just over 42% to less than 10%.
                    - SCHEDULER (IF USED)
                    - OPTIMIZER
                        
                        RMSProp
                            - Yields an average accuracy of around 53% with enhancing adjustments to loss function and 
                            learning rate.
                        Adagrad 
                            - Switching to the adagrad optimizer showed minimal improvements in average accuracy over 
                            RMSProp (the default optimizer for the project). 
                            - Average accuracy: 55%
                        Adadelta
                            - Yielded comparable results to RMSProp. Used same (optimal) learning rate of .00001 and a 
                            rho of .95.
                            - Average accuracy: 53%
                        Adam
                            - Yielded slightly better results than RMSProp. Used learning rate = .00001, beta_1 = 0.9, 
                            and beta_2=0.999
                            - Average accuracy: 56%
                        Adamax
                            - Average accuracy: 53%
                        Nadam
                            - Yielded highest average accuracy.
                            - Average accuracy: 60%
                    - EPOCH
                        - Increasing the number of epochs by a factor of 10 made a considerable improvement in the 
                        average accuracy.
                        - Average accuracy: 70%
                    - TRAIN SIZE
                    - TEST SIZE
                    - DATA DIMENSION HEIGHT X WIDTH
                    - NUMBER OF PARAMTERS OF YOUR MODEL [OPTIONAL]