# group_21_DSCI100_project

Hello, welcome to our group project!!

### Members
- Derek Wang (92116847)
- Ella Buric (76298694)
- Fernando Tabuchi (936534667)
- Sophie Juchymenko (80742364)

Predicting the Type of Chest Pain based on Age and Blood Pressure
 
Introduction:
 
Heart disease is an extremely prevalent health issue around the world. Angina is chest pain which is experienced by individuals who fail to get enough oxygen rich blood into parts of their heart muscle. Anginas can be a sign of coronary artery disease and a warning symptom of a heart attack. Angiography is an X-ray taken of the coronary arteries which is often used to diagnose heart disease. 
 
How do age and resting blood pressure influence the type of chest pain seen in patients admitted to the university hospitals in Zurich and Basel?
 
We will be using the heart disease dataset from the Switzerland database. This dataset contains a set of 14 variables; the data was collected from 143 patients undergoing angiography in university hospitals in Zurich and Basel. Chest pain type (cp) is described by 4 values:  1 is a typical angina, 2 is an atypical angina, 3 is non-anginal pain, and 4 is asymptomatic. Trestbps represents resting blood pressure and age represents the age of the patient.
 
Methods:
 
For this classification, we will use the predictive variables age and resting blood pressure to predict the type of chest pain seen in patients.

First we will load in the dataset, tidy it, and select for age, cp, and trestbps columns. We will split our data into training and testing sets, create a recipe, perform a cross-validation, create a K-nearest neighbors classifier, tune the model, and train the classifier with the training set via workflow. We will filter .metric for accuracy,  plot a neighbors vs. accuracy plot to visualize the best number of neighbors to set our final model. We will build a new K-nearest neighbors model with the ideal K value and run that through a workflow; this model will be used to predict the class for the test set (predict type of chest pain). 

One way we plan to visualize is to create a plot with the predictors on each axis and a different colour for each value of chest pain to visualize how the predictors can be used to predict the type of chest pain.
 
Expected Outcomes:
 
We expect to find that as age and resting blood pressure increases, the amount of cases of chest pain will increase especially those of typical angina and asymptomatic. As  age increases cardiac complications increase because arteries become less efficient which is correlated with chest pain.
 
These findings could be beneficial for better categorization of chest pain to help doctors correctly medicate a patient even if they wrongly, or cannot, describe the pain. For example, a patient could think he felt a typical angina, but due to his blood pressure and age he is predicted to have non-anginal type chest pain. In this case, the doctor could further examine the patient to make sure that he is given the correct medication.

Future question: Is one type of chest pain more likely to be linked to diagnosed heart disease? 

