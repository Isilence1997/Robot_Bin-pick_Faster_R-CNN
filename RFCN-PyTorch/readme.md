`requirements.txt 所需依赖
参考：https://github.com/elbert-xiao/Simple-RFCN-PyTorch
configs：存放配置文件
predict：imgs存放需要被检测的图片，results存放结果
训练好的网络：checkpoints
数据集约定格式：（VOC格式）

打开visdom
python -m visdom.server
开始训练
python train.py RFCN_train
评估
python train.py RFCN_eval --load_path='checkPoints/rfcn_voc07_0.725_ohem.pth' --test_num=5000
预测
python predict.py predict --load_path='checkPoints/rfcn_voc07_0.725_ohem.pth'

模型：checkPoints/rfcn_voc0712_0.768_ohem.pth