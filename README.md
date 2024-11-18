# RAFT
QT库遇到的问题
#在RAFT进行测试数据集的处理过程中，无法处理全部图像，报错显示有问题：

QMimeDatabase: Error loading internal MIME data
An error has been encountered at line 1 of <internal MIME data>: Premature end of document.:
解决方案：
安装 opencv-contrib-python 将解决该问题。
pip 安装 opencv-contrib-python
其他详细信息：Windows 10/x64 Python：3.10.9 Conda：23.1.0 Opencv：4.7.0 numpy：1.23.5 qt-main：5.15.2 pyqt：5.15.7 pyqt5-sip：12.11.0 qt-webengine：5.15.9 qtwebkit：5.212



RAFT在训练的时候出现报错

Traceback (most recent call last):
  File "train.py", line 17, in <module>
    from torch.utils.tensorboard import SummaryWriter
  File "C:\Users\PC\.conda\envs\RAFT\lib\site-packages\torch\utils\tensorboard\__init__.py", line 1, in <module>
    import tensorboard
ModuleNotFoundError: No module named 'tensorboard'

解决方案：
pip install tb-nightly
