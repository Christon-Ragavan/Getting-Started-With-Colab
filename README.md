# Getting Started With Google Colab


This following tutorial will get you started with using Google Colab. 
Google Colab can be interpreted as normal python notebook with added functionality. There are two general ways you can work with Colab.

1. Colab with Google Drive
2. Colab with Github mounting with google drive. (!!!Only if its private repository)

For now we can only use Colab with google drive which is really simple to get started. 

## A general overview of the steps involved 
1. You need to have a google account (or) create new one
2. Upload your scripts (Not data - To be extra careful about the copyrights comtent during traning)
3. Run the Scripts on Colab from Google Drive.



## Step 1: Setting Up
1. Create Google Account (or use Exsisting)
2. Click on "Add-on" with "+" sign which is towards the right-most column
![Add on](/images/setting_up_01.png)
3. Install Colabotory
![Install Colabotory](/images/setting_up_02.png)
3. Right Click and open a new colab file (.ipyb)
![newFIle](/images/setting_up_03.png)


## Step 2: Getting familier with Colab

1. Basically you can use it as jupiter notebooks. 
2. To install any packages use following:
```markdown
!pip install <package-name> 
 # Don't forget ! before pip. 
 # If you want to execute terminal commands use "!" before any desired terminal command
```
![usingcolab01](/images/colab_basics_01.png)

3. ** Set Run Time** - Go to Runtime>Change runtime type 
![usingcolab01](/images/colab_basics_02.png)


## Step 3: Run Scripts From Google Drive

In order to run a script you need to do following 3 steps
1. Mount your google drive with your .ipynb 
```markdown
from google.colab import drive
drive.mount('/content/drive')
```

2. You need to authorise which google drive you want to mount by signing in. After signing-in you will get a code which you can then paste it in the given area.(This can be done easily by following the instructions)

3. Go to the script location and run the script
```markdown
cd /content/drive/My Drive/Colab_with_g_Drive_tutorial
!python colab_test.py
```
![usingcolab01](/images/colab_basics_03.png)
```markdown
```

## General Tips:
1. Avoid uploading audio files in Google Drive, instead use extracted features (for example, spectogram saved as .npz file)
2. Google Colab notebooks have an idle timeout of 90 minutes and absolute timeout of 12 hours. This means, if user does not interact with his Google Colab notebook for more than 90 minutes, its instance is automatically terminated. Also, maximum lifetime of a Colab instance is 12 hours.
3. Try to avoid traning which takes longer than 12 hours (or break down your tranings)
4. There are way you can train the models online and save checkpoint in your google drive, check out some info [here](https://mc.ai/how-to-save-and-upload-deep-learning-machine-learning-models-in-google-colab-using-google-drive/)
5. If you want to use TPUs. check out some info  [here](https://www.dlology.com/blog/how-to-train-keras-model-x20-times-faster-with-tpu-for-free/)

## Some Basic Commands Needed

To check CPU and RAM specifications
```markdown
!cat /proc/cpuinfo
!cat /proc/meminfo
```


Check GPU specifications
```markdown
from tensorflow.python.client import device_lib
device_lib.list_local_devices()
```

For html link click [here](https://christon-ragavan.github.io/Getting-Started-With-Colab/)

