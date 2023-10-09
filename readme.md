Project stepwise explaination : 

Step1 :
creatingDataset.py

In this , date which is in the form of (dd-mm-yy) is categorized into 
seasons.

Only demand , availability, season , name, state is taken for training
purpose.
Dataset is created and dumped into the system using pickle.
Under the name (trainabledata.pickle)



Step2:

train.py

firstly , this program load the dumped trainabledata back to memory
then 

Train the RandomForestRegressor 
the model created is then dumped into the System using pickle under the name
(price_predictor_veg.pickle)



Step3:
app.py 

in this api is Created so that it can accept data from React App

then prediction is made on the using pythonScript.py module

Output is stored into the mongoDB Atlas.
Output is also shown in the React App


Why RandomForestRegressor?

Because my data set is too much random
to make best out of it Random Forest is used
as it ensemble decision tree.

Output of every decision tree is then go through
regression.

So , by this accuracy increases


data set is collected from Kaggle.com