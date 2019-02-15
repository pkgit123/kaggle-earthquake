# Kaggle Earthquake Competition
Exploring the Kaggle Earthquake Competition in Feb 2019.  I'm not planning to actually compete, but just familiarizing myself with the Kaggle Kernels (Jupyter Notebooks) and the kaggle-api command line interface. Based on some of the kernels I reviewed, noticed scikit-learn has some new libraries. Refreshing machine learning skills, most of my prior ML experience was during my master's degree.  

Tasks:
* Familiarize myself with Kaggle API (command line tool), use to download datasets.
* Unzip the datasets into folder.
* Move downloaded data into archive_folder to make it easier to follow.
* Update .gitignore file so not uploading huge datasets into github
* Read some public kernels and experiment with code in Juypyter Notebook.

1. Check out the LANL Earthquake Prediction page (https://www.kaggle.com/c/LANL-Earthquake-Prediction/data)
1. Check out the Kaggle API on github (https://github.com/Kaggle/kaggle-api)
	1. use the Kaggle API, sign up for a Kaggle account at https://www.kaggle.com. 
	1. Then go to the 'Account' tab of your user profile (https://www.kaggle.com/username/account) and select 'Create API Token'. This will trigger the download of kaggle.json, a file containing your API credentials. 
	1. Place this file in the location ~/.kaggle/kaggle.json (on Windows in the location C:\Users\<Windows-username>\.kaggle\kaggle.json - you can check the exact location, sans drive, with echo %HOMEPATH%). 
	1. You can define a shell environment variable KAGGLE_CONFIG_DIR to change this location to $KAGGLE_CONFIG_DIR/kaggle.json (on Windows it will be %KAGGLE_CONFIG_DIR%\kaggle.json).
1. Terminal commands for kaggle credentials, kaggle api cli, download data files
>
```shell
cd 
mkdir .kaggle  
mv ~/Downloads/kaggle.json ~/.kaggle/kaggle.json
cd ~/.kaggle/kaggle.json
subl kaggle.json
chmod 600 ~/.kaggle/kaggle.json
pip install kaggle
kaggle competitions download -c LANL-Earthquake-Prediction
```
>
1. It downloaded to home directory (~).
1. Move it to the kaggle directory manually (/Users/peterkim/Documents/personal-kaggle/earthquake)
1. Terminal commands
>
```shell
unzip train.csv.zip
unzip test.zip -d test_folder
```
>
1. Move zip files to an archive folder
1. Create a .gitignore file for the test_folder and the archive_folder
