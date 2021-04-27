<h1>Web Scraping</h1>

<h3>1. Import modules</h3>
chrome://version 에서 브라우저의 버전을 확인하고, 그에 맞는 chromedriver를 설치해야 한다.
<br></br>

```python
from selenium import webdriver
```
selenium 은 주로 Login , 페이지 이동 등 브라우저를 핸들링하는데 사용  
<br></br>

```python
from bs4 import BeautifulSoup
```
BeautifulSoup 은 웹페이지에 존재하는 태그에 접근해 필요한 내용을 추출
<br></br>

```python
import datetime
```
datetime 은 추후에 브라우저 이동 시간을 조절하기 위해 사용
<br></br>

```python
import time
```
time 은 실행 중 delay 걸리는 부분을 해소하기 위해 사용
<br></br>

```python
import pandas as pd
```
pandas 는 추출한 데이터를 DataFrame 형태로 만드는데 사용
<br>  </br>
<h3>2. headless 모드</h3>
```python
options = webdriver.ChromeOptions()
options.add_argument('headless')
options.add_argument('window-size=1920x1080')
options.add_argument("disable-gpu")

options.add_argument(
    "user-agent=Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/61.0.3163.100 Safari/537.36")


driver = webdriver.Chrome('chromedriver Route')

driver.implicitly_wait(5)
```
<br></br>

<h3>3. 
