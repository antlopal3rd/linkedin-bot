# linkedin-bot

A bot to automate connecting with people through Linkedin built on Selenium.

## Disclaimer:

Automating Linkedin activity goes against their terms of service. Although many measures have been taken to make this bot less prone to be detected it most likely will be at some point. This program is meant as an exercise.

## Setup:

The code uses an already registered user with their cookies so we don’t need to input the username and password every time. It also uses a modified version of the WebDriver in order to further avoid detection. If you already have a WebDriver you can open the file with a hex editor and change the word WebDriver and the string "cdc_adoQpoasnfa76pfcZLmcfl_" with something similar of the same length. This unique string is used by websites to detect if you are using selenium. To take this steps you can follow [this](https://themerkle.com/selenium-java-how-to-avoid-bot-detection-by-websites-when-using-chromedriver-exe/) guide.

If you don’t have the WebDriver yet installed you can use ChromeDriverManager which you can find [here](https://pypi.org/project/webdriver-manager/). To install it run the following code:
```
pip install webdriver-manager
```


