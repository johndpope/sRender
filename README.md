# sRender
We provide pytorch implementation for sRender.
# Sketch to Sketch result 
**left:** croquis style; **right:** charcoal style
![sketch2sketch](https://github.com/an0nym0u5-hackerese/srender/blob/main/images/sketch2sketch.png)
(a)sketch drawn by artists ; (b)line-drawings ; (c)systhesis sketch
# Photo to Sketch result
**left:** croquis style; **right:** charcoal style
![photo2sketch](https://github.com/an0nym0u5-hackerese/srender/blob/main/images/photo2sketch.png)
(a)photo ; (b)line-drawings ; (c)systhesis sketch
# Train and test
* charcoal_style for systhesising charcoal style images,it contains pip2pixHD for model without stroke_loss and with stroke_loss correspodingly
* croquis_style for systhesising croquis style images,it contains pix2pix,pix2pixHD and stroke
* download dataset [gray]() for **charcol_style**, [binary]() for **croquis_style**
* download pretrain model and put them in **./checkpoints** for test
* for model with stroke_loss,you should download [stroke_model](https://drive.google.com/drive/folders/1mvlSUN-A2RBzV27BZLvoc1OemwU9glwY) and specify model root in
**./models/pix2pixHD_model** for **net_c.load_state_dict**
* you can modify **options/base_option** to specify **--dataroot**, then run train.py or test.py
# Dataset
## gray  
* [charcoal](https://drive.google.com/drive/u/1/folders/1ZuRVlPwvtNtfkNIj-DIdi2kr-1kEcPhg?hl=zh-CN)
* [CelebAmaskHQ](https://drive.google.com/drive/u/1/folders/1ZuRVlPwvtNtfkNIj-DIdi2kr-1kEcPhg?hl=zh-CN)
* [FFHQ](https://drive.google.com/drive/u/1/folders/1ZuRVlPwvtNtfkNIj-DIdi2kr-1kEcPhg?hl=zh-CN)  
## binary 
* [croquis](https://drive.google.com/drive/u/1/folders/1VBUBdGWz324dhCu8LRFU5qB0PqXxNQIJ?hl=zh-CN)
* [CelebAmaskHQ](https://drive.google.com/drive/u/1/folders/1VBUBdGWz324dhCu8LRFU5qB0PqXxNQIJ?hl=zh-CN)
* [FFHQ](https://drive.google.com/drive/u/1/folders/1VBUBdGWz324dhCu8LRFU5qB0PqXxNQIJ?hl=zh-CN)  
# Pretrain model
## charcoal_style
* [pix2pixHD](https://drive.google.com/drive/u/1/folders/1-nnnt4qy8PkKRUJfAcK_o7sED3Ab5zCf?hl=zh-CN)
* [stroke](https://drive.google.com/drive/u/1/folders/1DHEe0QGcjAhwVHZ4qYafbSzCF_HoZ4n4?hl=zh-CN)  
## croquis_style
* [pix2pix](https://drive.google.com/drive/u/1/folders/1NIgo8U8UO43MH3KKnqFUXDcWTze_RWG4?hl=zh-CN)
* [pix2pixHD](https://drive.google.com/drive/u/1/folders/1NW6s5JKmnVIA-TX89QwB6ymjKXbDAmnL?hl=zh-CN)
* [stroke](https://drive.google.com/drive/u/1/folders/1c0xoDCpNbagxPfJUUmp1T0WrCZn7rfsB?hl=zh-CN)  
# Result
Our synthesis result for **croquis** and **charcoal** style can be downloaded
[Goole Drive](https://drive.google.com/drive/folders/1rDEe1GhBuoPUKDlj6kflfG1FTR6Xhu4u)
