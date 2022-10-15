# SBSPS-Challenge-9549-Develop-An-Accurate-Model-For-Cricket-Pose-Estimation
# Cricket Pose Estimation is a model - 
Used to predict the batting shots in images, videos or in livestreams.
Assist cricketers in analyzing their posture while playing for a Cricket shot and help them to monitor their pose after rehab.
It may also be used to maintain track of every player's performance in matches by monitoring their batting shot in relation to a certain baller and ball shot. It can then be used to assess each player's performance and help them become better via training. 
It may also be used to monitor the batting styles of the opposing team's players so that bowling and fielding strategies can be adjusted. 

# Model Description -
In order to construct this model, we constructed our own dataset and designed a Deep Learning Sequential LSTM model that follows Dense Layers at the end of the model by fine-tuning parameters to get better outcomes. We also utilized MediaPipe to keep track of body position.

# Main Technology Stack -
MediaPipe for Pose detection, Sequential, LSTM Model, Dense Layers, Anvil server 

# How to use - 
1. Download the code folder, upload it on jupyter notebook
2. open a new notebook and type command 'pip install anvil-uplink'R
3. Run 'main' python notebook.
4. Go to link - https://cricket-pose-estimation.anvil.app/
5. use 'username : admin' 'password : admin'.
6. Chose the specific option you want to go with, upload image/video or want to detect cricket pose via livestream.

# Presentation - 
https://docs.google.com/presentation/d/1lFDxPFsIes2Ur_sxeGVKMykgumzG1LBsN8nqszZ2h6w/edit?usp=sharing

# Dataset - 
1. Cricket pose video is the folder consiting of folders comprising videos of that specific shot
2. Preprocessing was done via 'preprocessing.ipynb' notebook , to convert the frames from these vides to .npy format and then use them again while model creation.
3. if you want to run 'preprocessing.ipynb' notebook to create dataset on your own , you will have to change the 'DATA_PATH' to the path where this folder is located in your system.
4. Else you can unzip 'After Preprocessing Dataset' folder , this folder consits of subfolders with specific pose name further comprising of files in .npy format carrying Pose keypoints extracted via MediaPipe.
5. If you want to run the 'MODEL.ipynb' notebook you will have to change 'DATA_PATH' to where your 'After Preprocessing Dataset' is located. 


