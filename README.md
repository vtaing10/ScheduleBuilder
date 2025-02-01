PyMongo Installation Guide
Prerequisites:
Python 3.6+ should be installed on your machine.
pip should be available for package installation.
Step 1: Verify Python Installation
Make sure Python is installed correctly. Open a terminal or PowerShell and type:

bash
Copy
Edit
python --version
If Python is installed, it will display the version number. If not, download Python here and install it, ensuring to check the box for Add Python to PATH.

Step 2: Install pip
If pip is not installed, follow these steps:

Download the get-pip.py script using curl or directly from this link.

Run the script to install pip:

bash
Copy
Edit
python get-pip.py
If you get a warning that pip.exe is not in your PATH, refer to Step 3 to fix the PATH issue.

Step 3: Add pip to PATH (if necessary)
If pip is installed but still not recognized in PowerShell or Command Prompt, follow these steps:

Locate the Scripts directory where pip.exe is installed. For example:

makefile
Copy
Edit
C:\Users\<YourUsername>\AppData\Local\Programs\Python\Python312\Scripts
Add this directory to your system's PATH:

Open Start, search for Environment Variables, and select Edit the system environment variables.
Click on Environment Variables.
Under User variables, find Path and click Edit.
Click New and add the directory where pip.exe is located.
Click OK to save.
Restart your terminal to apply the changes.

Step 4: Install PyMongo
Once pip is available, use the following command to install PyMongo:

bash
Copy
Edit
pip install pymongo
Alternatively, if pip isn't recognized in the terminal, navigate to the Scripts directory and use:

bash
Copy
Edit
.\pip install pymongo
Step 5: Verify Installation
After installing, verify that PyMongo is successfully installed by running the following Python script:

python
Copy
Edit
import pymongo
print(pymongo.__version__)
This should display the installed version of PyMongo.
