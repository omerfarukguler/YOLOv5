# yolov5

**Githup'dan yolov5'i alıp etkinleştirildi**

`!git clone https://github.com/ultralytics/yolov5  # clone`

`%cd yolov5`

`%pip install -qr requirements.txt  # install`
<br><br>

**Python'un bir kütüphanesi olan torch aktifleştirildi**

`import torch`

`from yolov5 import utils`

`display = utils.notebook_init()  # checks`
<br><br>

**coco128 dosyası açıldı. coco128 dosyalarını yolov5 ile bilgisayara görüntüler örneklendirildi.**

`!unzip -q ../coco128.zip -d ../`
<br><br>

`# Train YOLOv5s on COCO128`

`!python train.py --img 640 --batch 16 --epochs 3 --data coco128.yaml --weights yolov5s.pt --cache`
<br><br>

**Test için farklı görüntüler gösterildi**

`# TEST`

`!python detect.py --weights yolov5s.pt --img 640 --conf 0.25 --source coco128/images/val`
<br><br>

## Ve sonuç :)
![6adc0bde-a5cf-4603-b310-33342cfb7238](https://user-images.githubusercontent.com/73534224/146655531-bee48f4a-7114-4265-82b0-7f17b0550485.jpg)
<br>
![71230dc1-d8b7-411f-bd08-36a356455f49](https://user-images.githubusercontent.com/73534224/146655574-e749dcdd-0b68-48ed-ac98-2182e21d7b0a.jpg)

