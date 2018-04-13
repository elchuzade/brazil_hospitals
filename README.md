# brazil_hospitals

#### The dataset is about patients of hospitals in some of Brazil neighbourhoods. It comes from Kaggle.
### The goal is to predict whether the patient will Showup to the scheduled appointment or not

#### The labels are as follows
###### PatientId
###### AppointmentID
###### Gender
###### ScheduledDay
###### AppointmentDay
###### Age
###### Neighbourhood
###### Scholarship
###### Hipertension
###### Diabetes
###### Alcoholism
###### Handcap
###### SMS_received
###### No-show

##### Link to the dataset https://www.kaggle.com/joniarroba/noshowappointments/data

Firstly I have changed column names that were spelled wrong way, then deleted the rows that contained the wrong inputs that could affect the predictions. Then I hace changed date and time in the 'Scheduled', 'Appointment' columns and encoded all the string labels to integers. Next, I have filtered out all the columns that have not significant correlation with the prediction column (e.g. coorrelation coefficient < 0.001 and > -0.001). Finally I have used several classification methods such as MultnomianNB, Descision Tree,Random Forest and combination of Grid Search CV with Random Forest to predict the Showup status with around 80% accuracy.

##### Software used: Python, Jupyter-Notebook.
##### Libraries used: SkLearn, Pandas, Numpy, datetime.
