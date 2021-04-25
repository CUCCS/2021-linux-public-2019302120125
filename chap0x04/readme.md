## 第四次实验报告

#### 实验环境

1. Ubuntu 20.04
2. Visual Studio Code
3. Git bash

#### 实验要求

任务一：用bash编写一个图片批处理脚本，实现以下功能：

- - [x] 支持命令行参数方式使用不同功能

- - [x] 支持对指定目录下所有支持格式的图片文件进行批处理

- - [x] 支持以下常见图片批处理功能的单独使用或组合使用

  - [x] 支持对jpeg格式图片进行图片质量压缩

  - [x] 支持对jpeg/png/svg格式图片在保持原始宽高比的前提下压缩分辨率

  - [x] 支持对图片批量添加自定义文本水印

  - [x] 支持批量重命名（统一添加文件名前缀或后缀，不影响原始文件扩展名）

  - [x] 支持将png/svg图片统一转换为jpg格式图片

任务二：用bash编写一个文本批处理脚本，对以下附件分别进行批量处理完成相应的数据统计任务：

- [x] 统计不同年龄区间范围（20岁以下、[20-30]、30岁以上）的球员**数量**、**百分比**

- [x] 统计不同场上位置的球员**数量**、**百分比**

- [x] 名字最长的球员是谁？名字最短的球员是谁？

- [x] 年龄最大的球员是谁？年龄最小的球员是谁？

任务三：用bash编写一个文本批处理脚本，对以下附件分别进行批量处理完成相应的数据统计任务：

- [x] 统计访问来源主机TOP 100和分别对应出现的总次数

- [x] 统计访问来源主机TOP 100 IP和分别对应出现的总次数

- [x] 统计最频繁被访问的URL TOP 100

- [x] 统计不同响应状态码的出现次数和对应百分比

- [x] 分别统计不同4XX状态码对应的TOP 10 URL和对应出现的总次数

- [x] 给定URL输出TOP 100访问来源主机

#### 实验步骤

##### 任务一

1.在虚拟机中安装imagemagick

```bash
sudo apt-get update && sudo apt-get install imagemagick
```

2.编写代码

3.执行测试

##### 任务二

1.下载2014年世界杯运动员数据到本地，并放入要执行的文件夹

```bash
wget https://sec.cuc.edu.cn/huangwei/course/LinuxSysAdmin/exp/chap0x04
/worldcupplayerinfo.tsv
```

2.编写代码

3.执行测试

##### 任务三

1.将所需文件下载到本地并解压，执行下列语句

```
# 下载.7z文件
wget https://sec.cuc.edu.cn/huangwei/course/LinuxSysAdmin/exp/chap0x04/web_log.tsv.7z

# 安装p7zip： 
sudo apt-get install p7zip

# 解压缩文件： 
sudo p7zip -d web_log.tsv.7z
```

2.编写代码

3.执行测试



#### 参考资料

师哥/师姐实验报告 

https://github.com/CUCCS/linux-2020-LyuLumos/tree/ch0x04

https://github.com/CUCCS/linux-2019-xaZKX/tree/hw4/chap04