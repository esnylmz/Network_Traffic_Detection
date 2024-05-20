# Network_Traffic_Detection
Network Traffic and Intrusion Detection System with Data Mining Techniques Using the CIC-IDS2017 Dataset

## Authors
- Emine Esin YILMAZ-120200059
- Pınar Sude GÜRDAMAR-120103073
- Resul Erdem ARDUÇ-119200056
GROUP NO: 10, MTH410


### About the Dataset
The CIC-IDS2017 dataset is one of the important datasets for cybersecurity analysis. The CIC-IDS2017 dataset contains benign and six common attack network flows, which mirror the true real-world data (PCAPs). Additionally, it contains labeled flows based on timestamps, source and destination IP addresses, source and destination ports, protocols, and attack from the network traffic analysis performed using CICFlowMeter.

The obtained data set was stored in 8 different CSV files. These are drawn separately as working hours on Monday, working hours on Tuesday, working hours on Wednesday, morning working hours and afternoon working hours on Thursday, and both morning and afternoon working hours on Friday. Friday afternoon working hours appear in two ways: portscan and DDOS. 

Within the scope of this project, it is aimed to detect and classify cyber security threats by applying various data mining techniques on the CIC-IDS2017 dataset. 

### The link of the dataset is included below:
**https://www.kaggle.com/datasets/cicdataset/cicids2017**

### The Steps for Analyzing the Data and Training the Models
First, it is aimed to understand the data set. The preparation of the data set for application to the models was provided by preprocessing steps such as reducing the NaN values, eliminating the multiplexing data, downsampling for the equal distribution of label classes, digitizing the label column for the use of the model, and making correlation and feature selection. And our input data is ready!

<img width="920" alt="image" src="https://github.com/esnylmz/Network_Traffic_Detection/assets/102979440/32f4155d-d4d7-482b-9841-501bf44ce473">




Secondly, and explanatory data analysis was conducted on the processed data.


In the last step, 4 different classification models were trained and tested. With the RandomForestClassifier model, the correct detection of the network traffic data's type is achieved with an accuracy of 99%.


<img src="https://github.com/esnylmz/Network_Traffic_Detection/assets/102979440/598bd1c1-7f86-4e18-bbf0-dd2b1222e340" alt="table-chart" width="450"/>






# Opening the code with Google Colab Environment
Using Google Colab is one of the easiest ways you can use to open the code without installing any extra dependencies.

First, click the .ipynb file inside our repository. After that, you need to download the code. 
After downloading open Google Colab and click the "New Notebook" Tab that is visible on the top right of the page.

Then just browse through your files and add our .ipynb file 🙂

- To rerun the processes, the CSV file link is added here: https://www.kaggle.com/datasets/cicdataset/cicids2017

- You will click the download tab to download the 8 CSV files and they will be downloaded as archive.zip, inside the zip you can see the separate .csv files when you click the MachineLearning folder twice.

<img width="751" alt="image" src="https://github.com/esnylmz/Network_Traffic_Detection/assets/102979440/936c1e85-f434-4568-9406-9538e402e9e9">

- download that CSV file and when you open the code, click at the file shaped icon at the right menu, and drag the CSV files there (it is highlighted in the screenshot below):



<img width="434" alt="image" src="https://github.com/esnylmz/Network_Traffic_Detection/assets/102979440/c0696046-aaae-436b-b306-2ac634b539d3">



The code is ready for re-run, you can try and do all the things you want!! 🙂
Note: If an error occurs with the CSV files' paths, click on one of the separate files and select 'copy the path' and add that path inside the code:
- df1=pd.read_csv("The new path you copied")
- df2=pd.read_csv("The new path of CSV file 2 you copied")
                      .....
                      .....
                      .....



# Opening the code with the VSCode editor

->Requirements:
To run this project, the following software and libraries are required:
Python 3.x
Jupyter Notebook (VSCode) (Google Colab) (Kaggle)
Pandas
NumPy
Matplotlib
Seaborn
scikit-learn


->Installation:
Follow these steps to run the project:

->For best practice:
Create a new empty folder where you wat to download the project.

1.Open the terminal in your vscode editor. Inside the terminal, proceed with these codes below:

## Connect your computer to github:
 - git config --global user.name "Your Name"
 - git config --global user.email "your.email@example.com"

## Create a new folder then go to its path:
 - cd "Path of Your New Folder"

## Clone or download this project:
 
 - git clone https://github.com/esnylmz/Network_Traffic_Detection.git
 - cd Network_Traffic_Detection

## Install the required software and libraries if they're not already installed in your editor:
 
 - pip install pandas numpy matplotlib seaborn scikit-learn jupyter

Note: If there are any errors with the imports of the files, try to copy the paths of the files when you add to VsCode
It should look like this:

- df1=pd.read_csv("C:\\Users\\userX\Desktop\\abcdef\\Network_Traffic_Detection\\MachineLearningCSV\\MachineLearningCVE\\Monday-WorkingHours.pcap_ISCX.csv")
- df2=pd.read_csv("C:\\Users\\userX\\Desktop\\abcdef\\Network_Traffic_Detection\\MachineLearningCSV\\MachineLearningCVE\\Tuesday-WorkingHours.pcap_ISCX.csv")
- df3=pd.read_csv("C:\\Users\\userX\\Desktop\\abcdef\\Network_Traffic_Detection\\MachineLearningCSV\\MachineLearningCVE\\Wednesday-workingHours.pcap_ISCX.csv")



