# amazon_automation
# Name : S.Bala janani
# Reg no: 212223060027

# topic amazon_ atomation

# code

```
from selenium import webdriver
from selenium.webdriver.common.by import By
import time

driver = webdriver.Chrome()
driver.get("https:www.amazon.com/")
time.sleep(5)
login = driver.find_element(By.ID, "nav-link-accountList-nav-line-1").click()
time.sleep(5)
signin = driver.find_element(By.ID, "ap_email_login").send_keys("jananib510@gmail.com")
time.sleep(5)

dropdown = driver.find_element(
    By.CSS_SELECTOR,
    'span[data-action="a-dropdown-button"]'
)
dropdown.click()

time.sleep(5)
driver.find_element(By.XPATH, "//a[@role='option'][contains(@data-value,'\"IN\"')]").click()   # <-- changed line
time.sleep(5)
continue_button = driver.find_element(By.CLASS_NAME, "a-button-input").click()
time.sleep(5)
password = driver.find_element(By.ID, "ap_password").send_keys("Janani@2006")
time.sleep(3)
signin_button = driver.find_element(By.CLASS_NAME, "a-button-input").click()
time.sleep(100)
submit_button = driver.find_element(By.ID, "a-button-input").click()
time.sleep(10)
``` 
