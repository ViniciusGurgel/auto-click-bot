import time

from selenium import webdriver
from selenium.webdriver.chrome.options import Options
from selenium.webdriver.common.by import By
import pyautogui


options = Options()
options.add_argument("--window-size=1920,1080")
driver = webdriver.Chrome(options=options)
driver.get("https://www.ea.uniceub.br/Sistema/Acesso/Login")

Acesso = driver.find_element(By.NAME,"coAcesso")

Acesso.send_keys("Acesso")
time.sleep(1)
Senha = driver.find_element(By.NAME,"coSenha")

Senha.send_keys("Senha")
time.sleep(2)
Button = driver.find_element(By.ID,'btn-login').click()

time.sleep(10)
Y = 500
for x in range(5):
    pyautogui.moveTo(1380, Y)
    pyautogui.click()
    time.sleep(3)
    while driver.find_element(By.CLASS_NAME,'swiper-button-next'):
        pyautogui.moveTo(510, 630)
        pyautogui.click()
        time.sleep(1)
        button1 = driver.find_element(By.CLASS_NAME,'swiper-button-next').click()
        time.sleep(2)
        pyautogui.moveTo(900, 570)
        pyautogui.click()
        time.sleep(1)

    time.sleep(1)
    time.sleep(10)
    Y += 20

