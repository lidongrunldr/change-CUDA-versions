# change-CUDA-versions
在python的虚拟环境或服务器中更改cuda的版本

* 首先在控制台输入
```
vim ~/.bashrc 
```
* 现在就进入了`.bashrc`隐藏文件，接下来点`i`，进入编辑模式
* 然后将两处有cuda版本号的地方都改成项目需求版本，然后esc退出编辑
* 接下来在当前页面控制台的最下面输入
```
:wq
```
如果没有改动仅是查看则输入
```
:q！
```
然后回车
* 最后，在控制台中输入
```
source ~/.bashrc
```
进行重置。这一步会退出当前所在的虚拟环境，需要重新 
```
conda activate <环境名>
```
* 如果只是想要查看当前cuda版本，执行如下指令
```
nvcc -V
```
* 如果要查看当前显卡的占用，输入
```
nvidia-smi
```
* 查看当前服务器所有cuda版本
```
ls -l/usr/local | grep cuda
```
  
