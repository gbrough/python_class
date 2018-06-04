# Python Class
This is a small set of programs and set-up for a class on Python. Please feel free to use them.
## AWS setup
The class uses a Cloud9 AWS system. Instructions for this is available on AWS websites. Only a basic small system is needed.
Please see [AWS](https://aws.amazon.com). Please make sure that your root AWS account is not used when running Cloud9! Just setup a new Cloud9 small system. 
## Update Cloud9
Once you have the enviroment running, some code is needed. First run `git clone https://github.com/alohawild/python_class/` to get a copy of the programs.
### Get Conda
Conda is loaded from the terminal under the window in Cloud9. Remember Cloud9 is Linux.
```
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
chmod a+x Miniconda3-latest-Linux-x86_64.sh
./Miniconda3-latest-Linux-x86_64.sh
```
#### Enter and yes and y
When running the last command it will install `conda` and it has many prompts. The answer is always positive. Please ensure you do this right. If the command needs to run again then use a `-u` to update.
#### Close everything running!
It is critical to close all the running windows so that he changes will take affect. The `conda` command will run if it is installed and all running instance are stopped.
### The install
Just run these commands in a new window.
```
conda install numpy
conda install pandas
conda install scikit-learn
```
At this point the pi_calc.py program should run. 
### Install Google Finances
Use `pip install googlefinance.client` to install Google Finance. Again prompts are all postive.

### Drag contents
As this is UNIX (Linux) and thus there is no updated path. That means that the files and programs cannot find each other if run in the `Monte` diretory. You need to drag the `*.py` programs to the top folder and the CSV files too. 
# Example programs
There are a set of programs that are available to learn Python. Two are easy. Two are amazingly hard. One is given as an example of a possible improvement.
## Pi
The first program `py_calc.py` uses the numpy library for random number. It uses a Monte Carlo process to estimate the mathamatical value of pi. The comments explain how the program works. To outline, one can draw a circe in a box and randomly pick points and check if the point is in the circle. The ratio of success and failures is a form of pi. It is interesting that the method produces a weak result. It also shows you how fast your server is!
### Exercise
Run the program and notice its answer. Change the program to run for more less interations. The program will not improve its results much. The conclusion is not that the program is faulty, but that it relies on Python math and that is not that percise. The squareroot is also not needed as the code is for a box of size 1x1.
## Stock
The second program `NKE.py` uses the Google library to load a Python dataframe with the stock prices of a popular stock. The Google library also brings in the Python library `Pandas`.
### Exercise
Run the program. It displays a stock. All in minminal amount of data. The parameter is a Python dictionary that is used by the library to make the JSON calls to get the data. Change the stock to get a null value. Notice that you have to guess as the correct values. So far no documentaiton of the values has been discovered.
## Monte
This program is just nuts. Something written a few years ago before I knew Python that well. It works on a simple idea.
Take the dataset from the Kaggle.com site for the practise Titanic contest (see [Kaggle Titanic](
