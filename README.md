### **Introduction**
This git repository is created for cloud classification project. This project is implemented in two methods:
1. Standard CPU based - "cloud_combine.py" script is to train the DNN model for detecting cloudy pixels of Cross-track Infrared sounder using the top 75 Principal Components (PC)of it's spectrum.
2. GPU based


### **Software requirements**
1. Python 3.7 or above
2. Python IDE (Visual Studio Code)

### **Standard CPU-based implementation**

#### **I - Clone the repository**

#### **II - Set up the virtual environment**
1. Create a new folder and name it as cloudclassify.
2. Copy cloud_subpixel.py from cloned repository and place it inside cloudclassify folder.
3. In Visual Studio Code, go to Terminal and run the below in cmd terminal. This creates a virtual environment called "cloudclassify-venv"
   
            python -m venv cloudclassify-venv
4. For Windows, run below line to activate the virtual environment
   
            cloudclassify-venv\Scripts\activate.bat
#### **III - Install python packages**
      
            pip install TensorFlow scipy scikit-learn matplotlib       

#### **IV Download the data**
1. Click the [link](https://drive.google.com/drive/u/0/folders/1d9uS1EDtIkmTHu3pDhJgR7mbqVS2gZNM) and download the input data.
2. Place the downloaded "cloud_pc.sav" file inside cloudclassify folder

#### **V - Run the script**
Now, we are all set to run the script.

### **GPU-based implementation**

#### **I - Open Google Colab**
1. Go to the [link](https://colab.research.google.com/notebooks/intro.ipynb#recent=true).
2. Click on the Upload tab.
   ![image](https://github.com/stccenter/CloudClassification/blob/main/Images/GoogleColabUpload.png)
3. Choose the "CloudClassifyGPU.ipynb" downloaded from the Git repository.

#### **II - Download train and test data and upload them in your Google Drive**
1. Go to the [data link](https://drive.google.com/drive/folders/1XqrxJd6rGgd0N2QJXRd1fm5aCZiSZClR?usp=sharing).
2. Download all three folder to your local machine.
3. Then upload it to your Google drive.
4. Create a new folder called "logs" inside the same folder where you uploaded the above three folders.

#### **III - Mount the GDrive**
1. Now go to the CloudClassifyGPU.ipynb notebook.
2. Run the code block "Mount the Google drive".
3. Click on the URL.
    ![image](https://github.com/stccenter/CloudClassification/blob/main/Images/MountGdrive.PNG)
4. Obtain the authorization code and paste it in the "Enter your authorization code" box.
5. Verify Google drive is mounted correctly.
   1. Click file icon in the left panel.
   2. Click Mount Drive (third option).
   3. Click "Connect to Google Drive" when it asks for permission. It takes few minutes to mount.
   4. Once it is mounted, you should see drive folder. See screenshot below:
   ![image](https://github.com/stccenter/CloudClassification/blob/main/Images/VerifyGdrive.png)

#### **IV - Change Runtime to GPU**
1. Go to Runtime in menu.
2. Click "Change runtime type".
   ![image](https://github.com/stccenter/CloudClassification/blob/main/Images/ChangeRunTime.png)
3. In Notebook setting, change Hardware accelerator to "GPU" and click Save.
   ![image](https://github.com/stccenter/CloudClassification/blob/main/Images/RunTimeGPU.png)
   

#### **IV - Run the notebook**
