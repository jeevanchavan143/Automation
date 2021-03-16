from selenium import webdriver
import pickle

options = webdriver.ChromeOptions()
options.add_argument("start-maximized")
driver = webdriver.Chrome(options=options, executable_path=r'./chromedriver.exe')
driver.get("Google.com")
a=input("Enter PIN:")
pickle.dump( driver.get_cookies(),open("train.pkl","wb"))
print("Success")
