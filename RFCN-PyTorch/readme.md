### requirements.txt 所需依赖  
- refer：https://github.com/elbert-xiao/Simple-RFCN-PyTorch  
- configs：存放配置文件  
- predict：imgs存放images need to be detected
- trained networks：checkpoints  
- dataset format：（VOC格式）  

### open visdom  
```python -m visdom.server  ```

### train  
```python train.py RFCN_train  ```

### evaluate  
```python train.py RFCN_eval --load_path='checkPoints/rfcn_voc07_0.725_ohem.pth' --test_num=5000  ```

### predict  
```python predict.py predict --load_path='checkPoints/rfcn_voc07_0.725_ohem.pth'  ```

### model：checkPoints/rfcn_voc0712_0.768_ohem.pth  