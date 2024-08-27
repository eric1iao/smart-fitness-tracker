# Smart Fitness Tracker

## About

This is a machine learning model allowing users to classify barbell exercises and count repetitions through accelerometer and gyroscope data from a fitness watch device.

## Getting Started

### Prerequisites

- Anaconda
- Docker

Using Anaconda, you can run the code in your favorite IDE and install the SFT requirements in a separate virtual environment. Naturally, if you are familiar with virtual environments and requirements files one can choose the setup of your choice, but please be aware that this setup is not tested and you have to solve the problems you encounter yourself. Download and install Anaconda from: https://docs.anaconda.com/anaconda/install/

Clone the SFT repository by running:

```
git clone https://www.github.com/mhoogen/ML4QS.git](https://github.com/eric1iao/smart-fitness-tracker.git
```

Open the Anaconda Prompt as Adminstrator (when you right click on the Anaconda Prompt, you see the option 'as Adminstrator'). Run the following command:

```
$ conda create --name myenv python=3.8.8
$ conda activate myenv
```

Then, navigate back to the Python3Code folder using cd <path to your ML4QS/Python3Code folder>.

Run the following commands to install the required dependencies:
```
$ pip3 install -r requirements.txt
```
```
$ pip3 install -r requirements_git.txt
```

It could be the case that you run into an error when installing pybrain/pyflux. Two possible solutions are given here:

An error stating: '... error microsoft visual c++ 14.0 or greater is required'. In this case, you need to install Visual Studio Build Tools via the following link: https://visualstudio.microsoft.com/visual-cpp-build-tools/ . Once installed, you need to open it, click on modify and mark 'Desktop development with C++'. Afterwards, you might need to reboot. More information can be found via: https://docs.microsoft.com/en-us/answers/questions/136595/error-microsoft-visual-c-140-or-greater-is-require.html.

If there is a different pyflux error, installing pyflux via a wheel might help. Download a pyflux wheel (based on your python version and desktop) and pip install it in the current working directory.
Step 1: Download the pyflux wheel file. Pick the 32 or 64 file. Check your desktop settings (64 or 32).
Step 2: Put the wheel file in the current working directory
Step 3: Install the wheel with the following command:

```
$ pip install pyflux‑0.4.17‑cp38‑cp38‑win_amd64.whl
```

Or if you have a 32 desktop:
```
$ pip install pyflux‑0.4.17‑cp38‑cp38‑win32.whl
```

## Authors

* Eric Liao &mdash; [eric1iao](https://github.com/eric1iao)


## Errors

If you find an error (there are plenty) that's not already listed, please open a new [issue](https://github.com/eric1iao/smart-fitness-tracker/issues).

## Contributing

If you would like to contribute new features/material or by fixing errors, please fork the repository, make your changes, and open a pull request.

## Acknowledgements

I would like to thank Mark Hoogendoorn and Burkhardt Funk, the authors of [Machine Learning for the Quantified Self]([http://littleosbook.github.io/](https://link.springer.com/book/10.1007/978-3-319-66308-1)), whose tutorials I used to begin the project.

## License

This project is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html). Follow the link for more details.
