Installation and Setup
In order to make sure that the provided code runs on all platforms (Windows, Max and Linux). We strongly advise to make use of Anaconda (or Miniconda). Using Anaconda, you can run the code in your favorite IDE and install the ML4QS requirements in a separate virtual environment. Naturally, if you are familiar with virtual environments and requirements files one can choose the setup of your choice (Docker Start Up Guide Below), but please be aware that this setup is not tested and you have to solve the problems you encounter yourself. Download and install Anaconda from: https://docs.anaconda.com/anaconda/install/ Clone the ML4QS repository by running:

git clone https://www.github.com/mhoogen/ML4QS.git
Windows:
Open the Anaconda Prompt as Adminstrator (when you right click on the Anaconda Prompt, you see the option 'as Adminstrator'). Run the following command:

conda create --name myenv python=3.8.8
conda activate myenv
Then, navigate back to the Python3Code folder using cd <path to your ML4QS/Python3Code folder>.

Run the following commands to install the required dependencies:

pip3 install -r requirements.txt 
pip3 install -r requirements_git.txt 
It could be the case that you run into an error when installing pybrain/pyflux. Two possible solutions are given here:

An error stating: '... error microsoft visual c++ 14.0 or greater is required'. In this case, you need to install Visual Studio Build Tools via the following link: https://visualstudio.microsoft.com/visual-cpp-build-tools/ . Once installed, you need to open it, click on modify and mark 'Desktop development with C++'. Afterwards, you might need to reboot. More information can be found via: https://docs.microsoft.com/en-us/answers/questions/136595/error-microsoft-visual-c-140-or-greater-is-require.html.

If there is a different pyflux error, installing pyflux via a wheel might help. Download a pyflux wheel (based on your python version and desktop) and pip install it in the current working directory. Follow the steps to perform.
Step 1: Download the pyflux wheel file from this Github repository via the folder pyflux_wheel. There are two files in this folder. We work with python 3.8.8 so therefor the number 38 is in the file. You either pick the 32 or 64 file. Check your desktop settings (64 or 32). You can check that here
Step 2: Put the wheel file in the current working directory
Step 3: Install the wheel with the following command:

pip install pyflux‑0.4.17‑cp38‑cp38‑win_amd64.whl
Or if you have a 32 desktop:

pip install pyflux‑0.4.17‑cp38‑cp38‑win32.whl
