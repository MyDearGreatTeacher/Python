```
Python：網路爬蟲與資料分析入門實戰
作者： 林俊瑋, 林修博  
出版社：博碩
https://github.com/jwlin/web-crawler-tutorial
```

```
import requests
from bs4 import BeautifulSoup


def main():
    resp = requests.get('http://blog.castman.net/web-crawler-tutorial/ch1/connect.html')
    soup = BeautifulSoup(resp.text, 'html.parser')
    print(soup.find('h1').text)


if __name__ == '__main__':
    main()
```
