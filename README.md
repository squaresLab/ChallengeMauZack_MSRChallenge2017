# MSR-challenge-2017

Paper submitted to the MSR Challenge 2017: Analyzing the Impact of Social Attributes on Commit Integration Success

To compute the decision trees: (these steps are corerct for Weka version 3.6.14)
1. First, start the command line GUI with the arguments -m 10g to increase the  available memory to Weka (you may be able to get by with less but we didn't check). 
2. Then, click on the Explorer button.  
3. Then click open file and open the arff file that corresponds to the decision tree you want to generate in the repository file 'Scripts and datasets/DecisionTreesAndData.zip'. 
5. Next, click on the classify tab. 
6. Click the Choose button.   
7. Select 'trees/J48'. 
8. Finally, click start.


To compute the core team member results:
1. Convert the arff file to a CSV file (the arff files can be found in 'Scripts and datasets/DecisionTreeesAndData.zip' ); This can be done by removing all information from the @DATA line and above in the file.
2. Adjust the file name in line 3 of the script checkCorePassRate.py to the correct file to the new csv file.
3. Run the script with python 3. 

To compute the foller results:
1. Convert the arff file to a CSV file (the arff files can be found in 'Scripts and datasets/DecisionTreeesAndData.zip' ); This can be done by removing all information from the @DATA line and above in the file.
2. Adjust the file name in line 3 of the script testFollowers.py to the correct file to the new csv file.
3. Run the script with python 3. 
