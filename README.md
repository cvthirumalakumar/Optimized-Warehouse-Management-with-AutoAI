# SBSPS-Challenge-2688-Optimised-Warehouse-Management-with-AutoAI
IBM HACK CHALLENGE 2020:It is all about coding for a cause.It’s about finding solutions for the problems that are existing in the society and becoming difficult to face.

This projects is done as a part of IBM Hack Challenge 2020

##***Team Name : Challenging Coders

##***Contest : IBM Hack Challenge 2020

In this challenge we took the problem of Optimized Warehouse Management of Perishable Goods for a Food Delivery Company.

We provided the project documentation file in the repository please check that documentation file to know full details about the project.

Our User Interface link : https://node-red-sdrss.eu-gb.mybluemix.net/ui/

We made a video for demonstration of our entire project.
Youtube link for our video demonstration : https://youtu.be/j7WTdpjLSyk


Below is our project template to gain you some basic knowledge on our project.Please read documentation file for full details.
Project Template
Title: Optimised Warehouse Management with AutoAI
Problem Statement:
        A food delivery company has to face lot of problems with
Perishable raw materials.Mainly not able to predict the sufficient future demands for the company.Due to this there will be more risk of wastage of materials or leads to out of stock.In both cases the company has to face economical loss.So,there is a need for accurate prediction of demands.Old statistical methods needs to be developed by using the current technology for accurate predictions.
        
Solution:
Machine learning is the most trending and useful technology for business predictions. It has several advantages like more accuracy,automates forecast updates based on recent data,high data processing speed etc when compared to the existing methods.So,we prefer machine learning model as a suitable solution for the given problem.

##1.Project Scope and Schedule:-

###1.1 Project Scope:

   Understanding the Scope of work from the following points

Goal of the Project:
    The goal of this project is to predict the demanded raw materials for next 10 weeks or future.To reduce the economical loss by reducing the wastage of perishable raw materials and can attain profits by securing the needs for demand.

Objective of the Deliverables:

   Task: Collecting the historical data from the food company that contains details about the past orders and training the model with the data and validating the model.

Deliverable: A list containing the details about the requirement of raw materials for next  10 weeks.
Difficulty Level:No need of coding experience with AutoAI.Easy to deploy with Node-Red(Basic understanding of HTML is sufficient).
Business / Social Impact:-
Decreases economical loss by reducing the wastage of perishable raw materials.
Increases profits by predicting the required quantity of demanded raw materials.
Less human effort for prediction of demand.
Helps in business expansion.

* [Article](https://www.potential.com/articles/project-scope/) -  regarding Project scope


###1.2 Work Division and Scheduling:
    Division of total work into separate tasks and assigning the task works among the team members based on their work experiences and interests.Then assigning time for each task based on the complexity of the tasks.


##2.Collection of Data:-

###2.1 Collecting Data:
    Collection of required data is the primary task in any machine learning model.The size of the dataset matters in the accuracy of the model.And also it needs to have the required features which are essential for prediction.In this task we will collect/gather all the available data from Kaggle.We will separate the collected data as per our requirement.
    
https://www.kaggle.com/shashkhr25/food-demand-forecasting-challange/data  -  Data Source Kaggle Link

##3.Pre-processing data:-
    Description:Pre-processing of the collected data into required form to meet the project needs is also the big-milestone.In this milestone we will be dealing with the data-transformation and splitting data.The remaining pre-processings related to null data and erroneous data are not required as we are using AutoAI.

###3.1 Transforming Data:
    Transforming the collected raw data into required form.The collected data is  specifying total number of orders in specific centers in particular week.As we are predicting the number of orders for next 10 weeks.We are grouping the orders in the scale of 10 weeks(i.e.Summing up the total number of orders of first 10 weeks as 1st category and next 10 weeks as 2nd category and so on).Then it will be easy to predict the demand for next 10 weeks in single step.
###3.2 Splitting Data:
    Division of entire data set into training set and testing set.Training set will be fed to the model in training and test set will be used to test the model after training.AutoAI  will train the model with given data by splitting .But we are dividing the data to test the trained model manually with our hands.For this we need separate data.So,we are splitting the data before giving it to AutoAI.

##4.Setting up IBM Cloud Environment:-

###4.1 Creating IBM Cloud account:
    Creation of IBM Cloud account will be done in this activity.Lite account is sufficient to develop this model.The necessary steps for creating the IBM Cloud account are clearly mentioned in the documentation.Follow the reference links to know about the

Signing up process. 

https://www.youtube.com/watch?v=HBkY-Fs1d6E  - Youtube Video

https://cloud.ibm.com/registration  -  Registration page

https://cloud.ibm.com/docs/account?topic=account-signup  -  documentation on creating account
###4.2 Creating Cloud Object Storage Service:
    Storage service is essential to create and use the services in the cloud.So,we are creating the Cloud Object Storage Service to meet the storage needs for the necessary services.Follow the reference link to know more about Cloud Object Storage Service and it’s uses.
    
https://www.ibm.com/cloud/object-storage   -  Documentation on what is cloud Object Storage

https://www.youtube.com/watch?v=VEoj69V6Rfg   -  Youtube video on creating Cloud Object Storage Service

https://cloud.ibm.com/docs/cloud-object-storage/basics?topic=cloud-object-storage-provision  -Documentation on creating Cloud Object Storage

###4.3 Creating Machine Learning Service:
    Creation of Machine Learning Service,which is necessary to train the model with AutoAI in Watson Studio.Follow the reference link to know more about machine learning service and it’s creation steps.
    
https://www.youtube.com/watch?v=NmdjtezQMSM   -  Youtube video on Machine learning service

###4.4 Creating Watson Studio Service:
    Creation of Watson Studio Service.AutoAI model options are available in Watson Studio.To use those AI services,we need to create the Watson Studio service first.

https://developer.ibm.com/recipes/tutorials/create-an-ibm-watson-studio-project/  -   Documentation for creating IBM watson studio

###4.5 Creating Node-Red Service:
    Creation of Node-Red for developing the User Interface(UI) while deploying the model.Node-Red is the suitable option to develop required User Interface(UI) without any background of programming knowledge.
    
https://www.youtube.com/watch?v=eVHm9UIsbuI  -  Youtube video on creation of Node-Red

https://www.youtube.com/watch?v=iEadmCNb_hE   -  Youtube Video on creation,developing of application on Node-Red

##5.Building Model

###5.1 Creating Watson AutoAI Project:
    Creation of AutoAI project with necessary services like Cloud Object Storage and Machine Learning services,which were created previously.Cloud Object Storage is for storing the project belonging files in the cloud.And machine learning service for using the machine learning models and deployments.Follow the reference links to know more.

Reference link:
https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/autoai-build.html 

https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/autoai_example_binary_classifier.html#step1    -  Sample model on IBM AutoAI
###5.2 Adding Assets
    Uploading the test data set file into the project.Model will be trained with the file which is present in the cloud.So,we need to upload the necessary data set file into the cloud before initiating the training process.  

Reference link:
https://dataplatform.cloud.ibm.com/docs/content/wsj/manage-data/add-data-project.html

##6.Training and Testing model

###6.1 Training AutoAI Model:
    Initiating the AutoAI model training with appropriate preferences and choosing the uploaded data set file.Saving the model with the best algorithm chosen by AutoAI by comparing the performances of the algorithms as model and deploying for further testing.
    
https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/autoai_example_binary_classifier.html#step1 - Documentation on Training the AutoAI Model

https://www.youtube.com/watch?v=O5wqjk_GeJo   -  Youtube video on creating,training,testing and deployment of AutoAI


 ###6.2 Testing Model:
    Testing the deployed model with the test data set which is separated from the entire data set and observing the predicted results with actual values.And estimating the performance of the model.If performance of the model is not satisfying then we can go back to train the model with other suitable algorithms and can achieve best performance among the all the algorithms available in AutoAI.

https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/autoai_example_binary_classifier.html#step3  -  Documentation on Testing AutoAI
  
##7.Developing UI and Deployment

 ###7.1 Developing UI with Node-Red:
    Node-Red is a flow editor to develop the User Interface without any background programming knowledge.It is very easy to create and easily understandable.So,we chosen Node-Red service to develop the User Interface(UI) which is created previously in a suitable format.UI is created,which makes the user to interface with the trained model very easy.

https://developer.ibm.com/components/node-red/tutorials/how-to-create-a-node-red-starter-application/  -   Documentation on create node-red application


 ###7.2 Deploying the Model on UI:
    Deploying the model on created UI by generating required API credentials and connecting the UI with the deployed model.
    
https://www.youtube.com/watch?v=O5wqjk_GeJo-  -   Boot camp video on deployment
    

 7.3 Interfacing with UI:
    Verifying the final ready-to-use model and testing the model from User Interface(UI)(Accessing the final model through UI).Making necessary changes to the UI to make the user feel easy to access the model.And submitting the final model.
