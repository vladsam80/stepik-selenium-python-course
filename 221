from selenium import webdriver
from selenium.webdriver.support.ui import Select

link = "http://suninjuly.github.io/selects1.html"
browser = webdriver.Chrome()
browser.get(link)

int1 = browser.find_element_by_xpath("//span[@id='num1']").text
int2 = browser.find_element_by_xpath("//span[@id='num2']").text

select = Select(browser.find_element_by_tag_name("select"))
select.select_by_visible_text(str(int(int1)+int(int2)))

inputs = browser.find_element_by_xpath("//button[contains(text(), 'Отправить')]")
inputs.click()
