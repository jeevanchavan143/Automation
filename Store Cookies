from selenium import webdriver
import pickle

options = webdriver.ChromeOptions()
options.add_argument("start-maximized")
driver = webdriver.Chrome(options=options, executable_path=r'./chromedriver.exe')
driver.get('Google.com')
cookies = pickle.load(open("train.pkl", "rb"))
for cookie in cookies:
    driver.add_cookie(cookie)

driver.get('Google.com')
