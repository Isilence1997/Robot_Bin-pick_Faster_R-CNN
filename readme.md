**pre_model_weights**：pretrained para weights of vgg16，resnet101

### DATASET PREDEFINED FORMAT：（VOC format）
- *.xml:
Annotations of each image in the total train set, with one-to-one correspondence between the image name and the annotation file name

- ImageSets  
    - train.txt(Extract a part of the total training set as the trainset)   

    - val.txt(Extract a part of the total training set as the validation set)  

    - trainval.txt(Extract a part of the total training set as the train and validation txt)  
    - train_test.txt(Extract a part of the total training set as the test txt)  

    - test.txt(truely test set) 

- JPEGImages  
    - **resize_test**: The image after the minimum side is scaled to 600px in the actual test set  

    - **resize_train_test**:Extract a portion of the total training set as the test set and scale the image after the minimum edge is scaled to 600px   

    - **resize_trainval**: Extract a portion of the total training set as the image after the minimum edge is scaled to 600px in the training and validation sets  

    - **testing**:The original to the real test set images   

     - **training** :The original total training set image   


### R-FCN：RFCN-Pytorch
detailed in RFCN-Pytorch/readme.md

### Light_head_rcnn: 
detailed in light_head_rcnn/README.md
**Light_head_rcnn is our FINAL method**

### Exp_Result:
- process/: physical experiment steps are recorded as bin_pick_0x_rgb_res.jpg
- detection/: We resized all images and generated detection rectangles in res_resize_0x.txt
- rebbit/,plug/,candlestick/ : simulation detect results

### Train_Result:
