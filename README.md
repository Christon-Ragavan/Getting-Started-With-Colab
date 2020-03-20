# Getting Started With Google Colab


This following tutorial will get you started with using Google Colab. 
Google Colab can be interpreted as normal python notebook with added functionality. There are two general ways you can work with Colab.

1. Colab with Google Drive
2. Colab with Github mounting with google drive

For now we can only use Colab with google drive which is really simple to get started. 

## A gneral overview of the steps involved 
1. You need to have a google account (or) create new one
2. Upload your scripts (Not data - To be extrac careful about the copyrights comtent during traning)
3. Run the Scrits on Colab from Google Drive.



## Step 1: Setting Up
1. Create Google Account (or use Exsisting)
2. Click on "Add-on" with "+" sign which is towards the right-most column
![Add on](/images/setting_up_01.png)
3. Install Colabotory
![Install Colabotory](/images/setting_up_02.png)
3. Right Click and open a new colab file (.ipyb)
![newFIle](/images/setting_up_03.png)


## Step 2: Using Colab

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


## Step 2: Run Scripts From Google Drive

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


For html link click [here](https://christon-ragavan.github.io/Getting-Started-With-Colab/)

