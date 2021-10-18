# pytest-automation-framework
This is API automation framework using pytest with python.
  
![](https://github.com/shyedhu/images/blob/main/pytest.gif)

## Prerequisites

Please ensure you have python3 installed on your machine. If not already installed, you can go to https://www.python.org/downloads/ and download the latest version of python for your OS and run the installer

Alternatively if you are on mac/linux and have homebrew/linuxbrew already installed then you can install python using below command

```console

brew install python

```

please make sure python is installed and available from the command line

```console

python3 --version

```

# Install the requests and pytest 

```console

pip install -U requests

```

We also need a testing framework to provide us with a test runner, I selected the pytest

```console

pip install -U pytest

```


**1. ** Clone this repo locally:
```console

git clone https://github.com/shyedhu/pytest-automation-framework.git

```

To generate HTML reports with the Pytest framework we have to install a plugin. For the installation, we shall execute the command

```console

pip install pytest-html

```

# To Run PyTests in Parallel

```console

pip install pytest-xdist

```

## Running tests

navigate into the project folder

cd pytest-automation-framework

```console

python3 -m pytest tests/ --html=report.html

```

# Pytest - Run Tests in Parallel


```console

python3 -m pytest tests/ -n 3 --html=report.html

```
-n <num> runs the tests by using multiple workers, here it is 3.


# Test Execution Results in XML Format

```console

 python3 -m pytest tests/ --junitxml="result.xml"

```

# Run the Pytest with Grouping 

```console

python3 -m pytest tests/ -m regression --html=report.html

```

# Run Single test class

```console

python3 -m pytest tests/product_test.py --html=report.html

```

# Viewing the html test report, just navigate the report.html file on your browser

![](https://github.com/shyedhu/images/blob/main/pytest-report-html.png)
