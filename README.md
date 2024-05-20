# Network_Traffic_Detection
Network Traffic and Intrusion Detection System with Data Mining Techniques Using the CIC-IDS2017 Dataset

The CIC-IDS2017 dataset is one of the important datasets for cybersecurity analysis. The CIC-IDS2017 dataset contains benign and six common attack network flows, which mirror the true real-world data (PCAPs). Additionally, it contains labeled flows based on timestamps, source and destination IP addresses, source and destination ports, protocols, and attack from the network traffic analysis performed using CICFlowMeter.

The obtained data set was stored in 8 different CSV files. These are drawn separately as working hours on Monday, working hours on Tuesday, working hours on Wednesday, morning working hours and afternoon working hours on Thursday, and both morning and afternoon working hours on Friday. Friday afternoon working hours appear in two ways: portscan and DDOS. 

Within the scope of this project, it is aimed to detect and classify cyber security threats by applying various data mining techniques on the CIC-IDS2017 dataset. 

First, it is aimed to understand the data set. The preparation of the data set for application to the models was provided by preprocessing steps such as reducing the NaN values, eliminating the multiplexing data, downsampling for the equal distribution of label classes, digitizing the label column for the use of the model, and making correlation and feature selection. 

Secondly, and explanatory data analysis was conducted on the data.

In the last step, 4 different classification models were trained and tested. With the RandomForestClassifier model, the correct detection of the network traffic data's type is achieved with an accuracy of 99%.



# Opening the code with Google Colab Environment
Using Google Colab is one of the easiest ways you can use to open the code without installing any extra dependencies.

First, click the .ipynb file inside our repository. After that, you need to download the code. 
After downloading open Google Colab and click the "New Notebook" Tab that is visible on the top right of the page.

Then just browse through your files and add our .ipynb file 🙂

To rerun the processes, the CSV file link is added in the repo, download that CSV file and when you open the code, click at the file shaped icon at the right menu, and drag the CSV files there.



<img width="434" alt="image" src="https://github.com/esnylmz/Network_Traffic_Detection/assets/102979440/c0696046-aaae-436b-b306-2ac634b539d3">



The code is ready for re-run, you can try and do all the things you want!! 🙂
Note: If an error occurs with the CSV files' paths, click on one of the separate files and select 'copy the path' and add that path inside the code:
df1=pd.read_csv("The new path you copied")
df2=pd.read_csv("The new path of CSV file 2 you copied")
