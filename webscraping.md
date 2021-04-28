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

