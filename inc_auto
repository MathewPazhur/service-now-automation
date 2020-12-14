#Importing
from selenium import webdriver
from time import sleep
from selenium.webdriver.common.keys import Keys

def login(driver):                                                            #Login Function
    username = driver.find_element_by_id("UsernameInputTxt")                  #Replace UsernameInputTxt with id of username field
    password = driver.find_element_by_id("PasswordInput")                     #Replace PasswordInput with id of password field
    
    username.send_keys("username")
    password.send_keys("password")
    
    driver.find_element_by_name("btnSubmit").click()


c_options = Options()
c_options.add_argument("--start-maximized")                                                                                                 #Maximize window
driver = webdriver.Chrome(executable_path=r'C:\Users\path\to\chromedriver', options=c_options)
driver.get('<service cafe link here>')                                                                                                      #Open website
sleep(10)
login(driver)
sleep(20)

iframe = driver.find_element_by_id("gsft_main")                                                                                             #Wait for iframe to load 
driver.switch_to.frame(iframe)

#Business Service automation

b_service = driver.find_element_by_id("sys_display.incident.subcategory")
b_service.send_keys('CHOICE')
sleep(2)
b_service.send_keys(Keys.DOWN)
sleep(2)
b_service.send_keys(Keys.ENTER)


sleep(5)

#Subcategory automation

subcat = driver.find_element_by_id("sys_display.incident.u_subcategory")
subcat.send_keys('CHOICE')
sleep(2)
subcat.send_keys(Keys.DOWN)
sleep(2)
subcat.send_keys(Keys.ENTER)

sleep(5)

#Assiggnment group automation

a_group = driver.find_element_by_id("sys_display.incident.assignment_group")
a_group.send_keys('CHOICE')
a_group.send_keys(Keys.ENTER)














