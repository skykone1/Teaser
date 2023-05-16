#安装

1.进入dockerfile文件目录，然后运行dockerfile文件创建镜像

```python
cd /path_to_dockerfile

docker build -t df_teaser .
```

2.在portainer.io中用镜像创建容器，配置如下
![20230516162923](https://raw.githubusercontent.com/skykone1/images/main/20230516162923.png)

![20230516163233](https://raw.githubusercontent.com/skykone1/images/main/20230516163233.png)


![20230516163257](https://raw.githubusercontent.com/skykone1/images/main/20230516163257.png)

3.进入容器，手动安装pytorch=1.5.1带pytorch的版本  
```python
pip install -c local "/home/dingfei/dependences/pytorch-1.5.1-py3.6_cuda10.1.243_cudnn7.6.3_0.tar.bz2"
```

4.执行eval_teaser++文件  
```python
python /home/dingfei1/projects/teaser++/examples/teaser_python_fpfh_icp/eval_teaser.py
```

5.看到输出信息  
![20230516163714](https://raw.githubusercontent.com/skykone1/images/main/20230516163714.png)
