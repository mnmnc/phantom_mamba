# phantom_mamba
Headless interactions with web applications. Python + Selenium + PhantomJS


```python

from selenium import webdriver
driver = webdriver.PhantomJS(executable_path='D:\Apps\phantomjs\phantomjs.exe')

driver.set_window_size(1120, 550)
driver.get("https://duckduckgo.com/")
driver.save_screenshot("out.png")
driver.find_element_by_id('search_form_input_homepage').send_keys("realpython")
driver.find_element_by_id("search_button_homepage").click()
driver.save_screenshot("out2.png")
print(driver.current_url)
driver.quit()
```
