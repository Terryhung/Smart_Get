# Smart_Get
Automatically assign user agent and check encoding for html by charset.

## Dependences

* [requests](http://docs.python-requests.org/en/master/)
* [bs4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)

## Class
SmartGet
  - attributes:
    - ua: user-agent (default is FireFox pc)
  - methods:
    - run:
      - parameters:
        - link: target link
      - respond:
        - requests.Response

## Usage

```python
from smart_get.smart_get import SmartGet

url = 'https://guides.github.com/activities/hello-world/'

r = SmartGet(ua='your user agent')
resp = r.get(url)

```
