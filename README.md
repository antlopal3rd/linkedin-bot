# LINKEDIN-BOT

![alt text](https://img.icons8.com/ios/500/selenium-test-automation.png)

A bot to automate connecting with people through Linkedin built on Selenium.

## Disclaimer:

Automating Linkedin activity goes against their terms of service. Although many measures have been taken to make this bot less prone to be detected it most likely will be at some point. This program is meant as an exercise.

## Setup:

The code uses an already registered user with their cookies so we don’t need to input the username and password every time. It also uses a modified version of the WebDriver in order to further avoid detection. If you already have a WebDriver you can open the file with a hex editor and change the word WebDriver and the string "cdc_adoQpoasnfa76pfcZLmcfl_" with something similar of the same length. This unique string is used by websites to detect if you are using selenium. To take this steps you can follow [this](https://themerkle.com/selenium-java-how-to-avoid-bot-detection-by-websites-when-using-chromedriver-exe/) guide.

If you don’t have the WebDriver yet installed you can use ChromeDriverManager which you can find [here](https://pypi.org/project/webdriver-manager/). To install it run the following code:
```
pip install webdriver-manager
```
Once you have the driver installed you should run Selenium and go in Linkedin so your cookies are saved. After that you have to tell Selenium to always that usee that has the cookies saved. Just change this line:
```
opciones.add_argument(f"user-data-dir=C:\\Users\\{username}\\AppData\\Local\\Google\\Chrome\\User Data\\Profile 2")
```
Now you can modify, if you want, the webdriver according to the previous guide and tell Selenium to always use that one. To do that you can modify this line:
```
PATH = f'C:\\Users\\{username}\\.wdm\\drivers\\chromedriver\\win32\\105.0.5195\\chromedriver.exe'
```
You are all set!

## How to use the program:

Open the code and change this line to your linkedin profile:
```
initial_navigation("https://www.linkedin.com/in/williamhgates/")
```
Change this other line to your desired keywords:
```
search_bar("data analyst")
```
And last this line to your desired number of new contacts you wish:
```
people_to_add(20)
```
Good luck!







