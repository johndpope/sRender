# sRender
We provide pytorch implementation for sRender：Bridging Unpaired Facial Photos And Sketches By Line-drawings
# Reconstructed sketches 
**left:** croquis style; **right:** charcoal style
![Reconstructed sketches](https://github.com/an0nym0u5-hackerese/srender/blob/main/images/sketch2sketch.png)
(a)Sketches  ; (b)Generated Line-drawings ; (c)Synthesized Sketches
# Generated sketches
**left:** croquis style; **right:** charcoal style
![Generated sketches](https://github.com/an0nym0u5-hackerese/srender/blob/main/images/photo2sketch.png)
(a)Photos ; (b)Generated Line-drawings ; (c)Synthesized Sketches
# Train and test
* charcoal_style for systhesising charcoal style images,it contains **sRender w/o Lstr** for model without stroke_loss and **sRender** for model with stroke_loss correspodingly
* croquis_style for systhesising croquis style images,it contains **sRenderPix2Pix**,**sRender w/o Lstr** and **sRender**
* download dataset [gray](https://drive.google.com/drive/folders/1ZuRVlPwvtNtfkNIj-DIdi2kr-1kEcPhg?usp=sharing) for **charcol_style**, [binary](https://drive.google.com/drive/folders/1VBUBdGWz324dhCu8LRFU5qB0PqXxNQIJ?usp=sharing) for **croquis_style**
* download pretrain model and put them in **./checkpoints** for test
* for model with stroke_loss,you should download [stroke_model](https://drive.google.com/file/d/16gSERA3TbPVFyCvKGtNKtJrQaOsG8vmO/view?usp=sharing) and specify model root in
**./models/pix2pixHD_model** for **net_c.load_state_dict**
* you can modify **options/base_option** to specify **--dataroot**, then run train.py or test.py
# Dataset
## gray line-drawings for charcol_style from GooleDrive   
* [charcoal](https://drive.google.com/file/d/18MAVm-u0l4Rfh4Ct6bZRG1cNbKwQMgMt/view?usp=sharing)
* [CelebAmaskHQ](https://drive.google.com/file/d/16pOkZiaBrot9EeLvxBIqm_UTuI2GSjpA/view?usp=sharing)
* [FFHQ](https://drive.google.com/file/d/1mC0Vzf6TLD-77vtkzmfmVf3ZZXRlyOVb/view?usp=sharing)  
## binary line-drawings for croquis_style from GooleDrive    
* [croquis](https://drive.google.com/file/d/1EMzyVvJnYhmyBMnriymgfFd_WCaURfto/view?usp=sharing)
* [CelebAmaskHQ](https://drive.google.com/file/d/1euiF1197sOEa6_dM6qE4tPMt0V42Vn-6/view?usp=sharing)
* [FFHQ](https://drive.google.com/file/d/1uJQ5JGttXLfwmpH5LH0yH3bgs2oT7kTa/view?usp=sharing)  
# Pretrain model
## charcoal_style from GooleDrive   
* [sRender w/o Lstr](https://drive.google.com/file/d/1mwGiFpXfMlcUw-ksfsyVhUSKQWQJGC6p/view?usp=sharing)
* [sRender](https://drive.google.com/file/d/1tRNzj2WSwITltKNxusfizO868_bdZ6Zq/view?usp=sharing)  
## croquis_style from GooleDrive   
* [sRenderPix2Pix](https://drive.google.com/file/d/1GIRcc8q-plIXKxSDEug4UMXacB35w0G5/view?usp=sharing)
* [sRender w/o Lstr](https://drive.google.com/file/d/1JdVhJDVCcFQ1jtNfNy-Q05UL4IVqkqw3/view?usp=sharing)
* [sRender](https://drive.google.com/file/d/1E7nqNeiC8I-FWYhtvcZHNdt0-7hWVF5g/view?usp=sharing)  
# Result
* Our synthesis result for **croquis** and **charcoal** style can be downloaded
[Goole Drive](https://drive.google.com/drive/folders/1rDEe1GhBuoPUKDlj6kflfG1FTR6Xhu4u?usp=sharing)
# Acknowledgments
* Our code is inspired by the [NVIDIA/pix2pixHD](https://github.com/NVIDIA/pix2pixHD) repository.
