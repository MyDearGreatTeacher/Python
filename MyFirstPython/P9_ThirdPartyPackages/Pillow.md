# Pillow函式庫/套件/模組(Python3)

>* https://pillow.readthedocs.io/en/5.1.x/

##### PIL(Python2) vs  Pillow(Python3)

>* PIL(Python Imaging Library)是Python平臺上的影像處理標準庫。PIL功能非常強大，但API卻非常簡單易用。PIL僅支持到Python 2.7
>* 一群志願者在PIL的基礎上創建了相容的版本，名字叫Pillow，支持最新Python 3.x，加入了許多新特性

安装Pillow==>sudo pip install pillow

https://pillow.readthedocs.io/en/5.1.x/reference/Image.html

PIL.Image.open(fp, mode='r')


##### 應用範例:圖片模糊特效
```
from PIL import Image, ImageFilter

# 打開一個jpg影像檔，注意是在當前路徑:
im = Image.open('cat.png')

# 應用模糊濾鏡filter():
im2 = im.filter(ImageFilter.BLUR)

# 將模糊濾鏡後的圖片存檔:
im2.save('cat_blur.jpg', 'jpeg')
```

### 應用範例:圖片縮放特效Create thumbnails

```
The following script creates nice thumbnails of all JPEG images in the current directory 
preserving aspect ratios with 128x128 max resolution.

from PIL import Image
import glob, os

size = 128, 128

for infile in glob.glob("*.jpg"):
    file, ext = os.path.splitext(infile)
    im = Image.open(infile)
    im.thumbnail(size)
    im.save(file + ".thumbnail", "JPEG")
```
##### 應用範例:圖片縮放特效
```
from PIL import Image

# 打開一個jpg影像檔，注意是當前路徑:
im = Image.open('cat.png')

# 獲得圖像尺寸:
w, h = im.size
print('Original image size: %sx%s' % (w, h))

# 縮放到50%:
im.thumbnail((w//2, h//2))
print('Resize image to: %sx%s' % (w//2, h//2))

# 把縮放後的圖像用jpeg格式保存:
im.save('cat_thumbnail.jpg', 'jpeg')
```

##### 應用範例:產生字母驗證碼圖片

先到底下下載自型 https://github.com/JotJunior/PHP-Boleto-ZF2/blob/master/public/assets/fonts/arial.ttf

存到目錄底下

```
from PIL import Image, ImageDraw, ImageFont, ImageFilter

import random

# 隨機字母:
def rndChar():
    return chr(random.randint(65, 90))

# 隨機顏色1:
def rndColor():
    return (random.randint(64, 255), random.randint(64, 255), random.randint(64, 255))

# 隨機顏色2:
def rndColor2():
    return (random.randint(32, 127), random.randint(32, 127), random.randint(32, 127))

# 240 x 60:
width = 60 * 4
height = 60
image = Image.new('RGB', (width, height), (255, 255, 255))

# 創建Font對象:
font = ImageFont.truetype('rial.ttf', 36)

# 創建Draw對象:
draw = ImageDraw.Draw(image)

# 填充每個圖元:
for x in range(width):
    for y in range(height):
        draw.point((x, y), fill=rndColor())

# 輸出文字:
for t in range(4):
    draw.text((60 * t + 10, 10), rndChar(), font=font, fill=rndColor2())

# 模糊:
image = image.filter(ImageFilter.BLUR)

image.save('code.jpg', 'jpeg')

```
