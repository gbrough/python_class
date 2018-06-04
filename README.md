# Python Class
This is a small set of programs and set-up for a class on Python.
# AWS setup
The class uses a Cloud9 AWS system. Instructions for this is available on AWS websites. Only a basic small system is needed.
Please see [AWS](https://aws.amazon.com). Please make sure that your root AWS account is not used when running Cloud9!
## Update Cloud9
First run `git clone https://github.com/alohawild/python_class/` to get a copy of the programs.
### Get Conda
```
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
chmod a+x Miniconda3-latest-Linux-x86_64.sh
./Miniconda3-latest-Linux-x86_64.sh
```
conda install numpy
conda install pandas
conda install scikit-learn
Use 'pip install googlefinance.client' to install Google Finance

Close cloud9 and then reopen from console to reset to new Python.
