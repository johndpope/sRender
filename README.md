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
* download dataset gray for charcol_style, binary for croquis_style
* download pretrain model and put them in ./checkpoints for test
* you can modify options/base_option to specify --dataroot, then run train.py or test.py
# Dataset
* gray
* binary
# Pretrain model
* charcoal_style
* croquis_style
# Result
Our synthesis result for croquis and charcoal style can be downloaded  
[result](https://drive.google.com/drive/folders/1rDEe1GhBuoPUKDlj6kflfG1FTR6Xhu4u)
