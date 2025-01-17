# Test Automation using Robot Framework with Selenium Library

This is a simple sample for Test Automation using [Robot Framework](https://robotframework.org/) with Selenium Library.


## Requirements

1. Install [VS Code](https://code.visualstudio.com/) or any Code Editor you're comfort with.
2. Install [python](https://www.python.org/), preferably version **3.9.10** (that's the one I used and having no issue).
3. Make sure `pip` also installed together with python. If it is not automatically installed, refer to [Python Crash Course](https://ehmatthes.github.io/pcc/chapter_12/installing_pip.html).
4. Update python to your PATH file. Refer [here](https://realpython.com/add-python-to-path/), this website covered configuration for Windows, Linux, and MacOS. Or, if you prefer using python version management tools, refer to [this article](https://medium.com/@zorozeri/how-to-install-pyenv-and-manage-pythonversion-on-your-local-machine-241b119b7ae9) for using [pyenv](https://github.com/pyenv/pyenv).
5. Download and open this code repository on your local Code Editor and run this command :
   ```
   pip install -r requirements.txt
   ```
   If the pip process is failed, try to downgrade your python version. I used python `3.9.10` when creating this repository (that's why I suggest it on requirements above). When I tried on different local machine with python `3.13.0` somehow the pip process is error.

## Run Tests
* Run all tests : 
   ```
   robot tests
   ```

* Run specific test : 
   ```
   robot tests/{test file name using extension ".robot"}

   sample :
   robot tests/001.robot
   robot tests/002.robot
   robot tests/LoginPageTest.robot
   ```

## Open Test Report
   MacOs : 

    open report.html
   Windows : 

    start report.html
   Or just drag and drop file `report.html` into your Browser.

## Open Test Log
   MacOs : 

    open log.html
   Windows : 

    start log.html
   Or just drag and drop file `log.html` into your Browser.

## Short Repository Explanation

This sample Test Automation consists of 4 main folders : 

* config
   ```
   Contains basic configuration of Variables, Settings, and Keyword wich will be used globally on this whole project
   ```
* log
   ```
   This folder will be filled with screenshot and logs from test execution, with one initial .txt file as placeholder only
   ```
* resources
   ```
   Consists of 3 more folders :
   > helpers  : contains any action which might be used globally on any pages
   > locators : contains web element for each specific web pages
   > pages    : contains actions which will be performed on each specific web pages
   ```
* tests
   ```
   Contains test cases
   ```

Apart from these 4 folders, this sample also using `env.yaml` file which can be used to store configuration-specific data. On this sample, URL for test is stored there :
   ```
   SauceDemo_URL: https://www.saucedemo.com/
   ```

## Selenium Library Keywords Documentation

https://robotframework.org/SeleniumLibrary/SeleniumLibrary.html

