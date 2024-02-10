### EX1 Creation of Employee, Weather dataset in WEKA Data Mining and Analysis Tool and perform Preprocessing
### DATE: 
### AIM: 
  To Create Employee, Weather dataset in WEKA Data Mining and Analysis Tool and perform preprocessing
### PROCEDURE: 
1) Open Start -> Programs -> Accessories -> Notepad
2) Type the following training data set with the help of Notepad for Employee Table.

```
--------------
Employee Data
---------------
@relation employee 
@attribute name {tevin,sarah,nithin,annie,jeffrey} 
@attribute id numeric
@attribute salary {low,medium,high} 
@attribute exp numeric
@attribute gender {male,female}
@attribute phone numeric

@data 
tevin,101,low,2,male,250311 
sarah,102,high,3,female,251665 
nithin,103,medium,1,male,240238 
annie,104,low,5,female,200200 
jeffrey,105,high,2,male,240240


--------------
Weather Data
---------------
@relation weather
@attribute outlook {sunny,rainy,overcast}
@attribute temparature numeric 
@attribute humidity numeric
@attribute windy {true,false} 
@attribute play {yes,no}

@data 
sunny,85.0,85.0,false,no 
sunny,83.0,86.0,false,no 
rainy,70.0,86.0,false,yes 
rainy,68.0,80.0,false,no
sunny,72.0,95.0,true,no 
sunny,69.0,70.0,false,yes 
rainy,65.0,70.0,true,yes
overcast,64.0,65.0,false,yes 
rainy,75.0,80.0,true,yes
overcast,80.0,90.0,false,no 

```
3) After that the file is saved with .arff file format.
4) Minimize the arff file and then open Start -> Programs -> weka-3-4.
5) Click on weka-3-4, then Weka dialog box is displayed on the screen.
6) In that dialog box there are four modes, click on explorer.
7) Explorer shows many options. In that click on ‘open file’ and select the arff file
8) Click on edit button which shows employee table on weka.

### OUTPUT:
Training Data Set -> Employee Table
![image](https://github.com/Evangelin-Ruth/WDM_EXP1/assets/94219798/202dc16c-8ba4-4755-89ed-723a8bcc1073)

Training Data Set-> Weather Table
![image](https://github.com/Evangelin-Ruth/WDM_EXP1/assets/94219798/5fbc2c6b-d2f2-4179-8101-375e6215e1bf)


### PREPROCESSING
### Procedure:
#### 1) Add -> Pre-Processing Technique:
1) Start -> Programs -> Weka-3-4 -> Weka-3-4
2) Click on explorer.
3) Click on open file.
4) Select Weather.arff file and click on open.
5) Click on Choose button and select the Filters option.
6) In Filters, we have Supervised and Unsupervised data.
7) Click on Unsupervised data.
8) Select the attribute Add.
9) A new window is opened.
10) In that we enter attribute index, type, data format, nominal label values for Climate.
11) Click on OK.
12) Press the Apply button, then a new attribute is added to the Weather Table.
13) Save the file.
14) Click on the Edit button, it shows a new Weather Table on Weka.

### OUTPUT:
Employee Table after adding new attribute ADDRESS
![image](https://github.com/Evangelin-Ruth/WDM_EXP1/assets/94219798/b1d26f1f-9ba3-45e7-92c3-30649bca2d53)

Weather Table after adding new attribute CLIMATE:
![image](https://github.com/Evangelin-Ruth/WDM_EXP1/assets/94219798/fce36e7a-9fc3-41e4-9840-9d974d3a2ca7)


### 2) Remove -> Pre-Processing Technique:

1) Start -> Programs -> Weka-3-4 -> Weka-3-4
2) Click on explorer.
3) Click on open file.
4) Select Weather.arff file and click on open.
5) Click on Choose button and select the Filters option.
6) In Filters, we have Supervised and Unsupervised data.
7) Click on Unsupervised data.
8) Select the attribute Remove.
9) Select the attributes windy, play to Remove.
10) Click Remove button and then Save.
11) Click on the Edit button, it shows a new Weather Table on Weka.

### OUTPUT:
Employee Table after removing attributes SALARY, GENDER:

![image](https://github.com/Evangelin-Ruth/WDM_EXP1/assets/94219798/a7fb4c64-7c00-4c5e-b9d6-543d677f1709)

Weather Table after removing attributes WINDY, PLAY:
![image](https://github.com/Evangelin-Ruth/WDM_EXP1/assets/94219798/c75e874d-ad97-4b14-a66f-2cd158b7a37e)


### Normalize -> Pre-Processing Technique:

1) Start -> Programs -> Weka-3-4 -> Weka-3-4
2) Click on explorer.
3) Click on open file.
4) Select Weather.arff file and click on open.
5) Click on Choose button and select the Filters option.
6) In Filters, we have Supervised and Unsupervised data.
7) Click on Unsupervised data.
8) Select the attribute Normalize.
9) Select the attributes temparature, humidity to Normalize.
10) Click on Apply button and then Save.
11) Click on the Edit button, it shows a new Weather Table with normalized values on Weka.

### OUTPUT:
Employee Table after Normalizing ID, EXP, PHONE:
![Uploading image.png…]()

Weather Table after Normalizing TEMPARATURE, HUMIDITY:
![Uploading image.png…]()

### RESULT: 
  Thus the program for generating employee and weather datasets has been developed, and preprocessing has been accomplished successfully.
