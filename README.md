# CircumSpect
Open-source software for processing images and generating natural language descriptions. Analyzes visual content using state-of-the-art computer vision algorithms. Suitable for researchers, programmers and anyone who needs quick understanding of image content.

#Prerequisites
  Python 3 - The code is entirely dependant on python
  NVIDIA GPU - It has to be NVIDIA in order to work
  Internet connection to download the required files and dataset
  At least 30GB of storage

# Installation
There are two ways to run this program: running the source code or downloading the installation app (only available for Windows YET).

If on Windows, you can either run the windows.py file or download the .exe file and run it by giving permission to run on your system, either way it will be the same. And on Mac or Linux you will need to run the linux.py file using python.

After executing the software, it will start downloading a library called Apex from NVIDIA -> https://github.com/NVIDIA/apex. This will only work if you have an NVIDIA GPU. After it attempts to download, a dialogue will appear asking you whether the Apex library has been installed properly without errors. And you can verify that be looking the messages above the dialogue. You can press enter if it says that Apex was installed successfully, if it says that there is an error in red text, that means Apex was not installed properly, and you need to I guess just figure it out because I haven't got to access to a GPU yet. 

Next it will install nlg-eval library, again asking whether it was installed successfully. It should most likely work, and you should be able to continue with the installation.

Now it will start downloading the image dataset that it needs to train off of. It will ask for credentials which you can just copy and paste from the message that is above it. When you paste the key in, it will not be visible but will be pasted in terminal, so DON'T KEEP PASTING IT IN CONSTANTLY. The dataset is around 14GB, but you still need about 30GB of storage available on your device because it first downloads a zipped file of the dataset, then unzips it taking double the storage. Don't worry, it will delete the zipped file itself, and if it somehow fails to do so, you can do it manually. If an image of zebras appear on the screen, the installation was successful and you can press enter to proceed with further installation.

This is the last part... a dialogue will now appear asking you whether you want to download the region_descriptions.json file. This is a necessary file for the software to understand where the parts of image are and their descriptions. You can press "y" and enter if you want to download it or "n" if you already have it somehow or want to modify something yourself. You will still need to have the file named as "region_descriptions.json" in the installation folder. There are chances that it will fail to install the file, so you can download it manually from the link it provides.

Now the program will work all by itself and you can sit back and relax until the installation finishes. All it will do is process the dataset and train the model it will work from.

#Usage
You can now type "description.py --help" to see all the commands. Or just directly type "description.py --img_path " followed by the path to the image you want to describe.
