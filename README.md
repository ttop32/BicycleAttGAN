# BicycleAttGAN
combine BicycleGAN and AttGAN


# Model structure

# TODO
- Resnet
- Vae
- latent input
- 

# Result   
![result](doc/screenshot_1.png)    
![result](doc/screenshot_2.png)     
![result](doc/screenshot_3.png)    
![result](doc/screenshot_4.png)    


# Run    



# Data Preparation
- Option 1: [CelebA](http://openaccess.thecvf.com/content_iccv_2015/papers/Liu_Deep_Learning_Face_ICCV_2015_paper.pdf)-unaligned (higher quality than the aligned data, 10.2GB)

        - download the dataset

            - img_celeba.7z (move to **./data/img_celeba/img_celeba.7z**): [Google Drive](https://drive.google.com/drive/folders/0B7EVK8r0v71pTUZsaXdaSnZBZzg) or [Baidu Netdisk](https://pan.baidu.com/s/1CRxxhoQ97A5qbsKO7iaAJg) (password rp0s)

            - annotations.zip (move to **./data/img_celeba/annotations.zip**): [Google Drive](https://drive.google.com/file/d/1xd-d1WRnbt3yJnwh5ORGZI3g-YS-fKM9/view?usp=sharing)

        - unzip and process the data

            ```console
            7z x ./data/img_celeba/img_celeba.7z/img_celeba.7z.001 -o./data/img_celeba/

            unzip ./data/img_celeba/annotations.zip -d ./data/img_celeba/

            python ./scripts/align.py
            ```


# Acknowledgement and References  
- [AttGAN](https://github.com/LynnHo/AttGAN-Tensorflow)     
- [EigenGAN](https://github.com/LynnHo/EigenGAN-Tensorflow)     
- [BicycleGAN](https://github.com/junyanz/BicycleGAN)
- [BicycleGAN-Tensorflow](https://github.com/clvrai/BicycleGAN-Tensorflow)
- [Bidirectional-InfoGAN](https://github.com/tohinz/Bidirectional-InfoGAN)
