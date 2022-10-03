# Abdulrahman Mahmoud's portfolio

# [Project 1: Facial recognition based attendance monitoring system](https://github.com/phdamg/phdamg.github.io)

This project is conducted for an HE institution with tens of thousands of students. The traditional method of attendance marking is a tedious task in many schools and colleges. It is also an extra burden to the faculties who should mark the attendance by manually calling the names of students which might take about 5 minutes of the entire session. Face recognition has set an important biometric feature, which can be easily acquirable and is non-intrusive. Face verification is a 1:1 matching process, it compares face images against the template face images and face identification is a 1:N problem that compares query face images. The purpose of this system is to build an attendance system that is based on face recognition techniques. Hence, the face of an individual will be considered for marking attendance.

Finalized approach
With a dataset of stored labelled faces
1.	Encode faces
2.	Detect a face using mediapipe, which detects a face in 0.01s
3.	Use the face_recognition library to identify the face, which has a 99.38% accracy.
4.	Find the person’s name from the encoding. 
5.  Store the persons name and time in a database.

![image](https://user-images.githubusercontent.com/114836975/193611560-5423d7f7-76c1-4622-896e-ffa99c526c53.png)
![image](https://user-images.githubusercontent.com/114836975/193612294-a03fbda3-7796-4389-88aa-5a3795680ef2.png)





# [Project 2: Data Science Salary Estimator](https://github.com/phdamg/phdamg.github.io)
* Created a tool that estimates data science salaries (MAE ~ $ 11K) to help data scientists negotiate their income when they get a job.
* Scraped over 1000 job descriptions from glassdoor using python and selenium
* Engineered features from the text of each job description to quantify the value companies put on python, excel, aws, and spark. 
* Optimized Linear, Lasso, and Random Forest Regressors using GridsearchCV to reach the best model. 
* Built a client facing API using flask 

![](/images/positions_by_state.png)


# [Project 2: Ball Image Classifier](https://github.com/phdamg/phdamg.github.io) 
For this example project I built a ball classifier to identify balls from different sports. This could be useful for someone who is new to sports from a certain country. They could take a picture of a ball and an app could serve them some information about the history and rules of the game. This is the underlying model for building something with those capabilities. 

I was able to get the model to predict the sport of the ball with 94% accuracy after minimal tuning. For most of the cases this would meet the need of an end user of the app. To get these results I used transfer learning on a CNN trained on resnet34. This created time efficiencies and solid results.

![](/images/matrix_results.png)
