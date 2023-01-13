1、提升Miner速度
2、优化CPU占用
3、修复网络错误的问题
(2)
4、修复提示libcudart.so缺失问题
5、优化Miner速度，3080 2.5k/s
(3)
6、修复2x系兼容问题
7、增加HiveOS支持
https://d15fsu2rilb7jj.cloudfront.net/hpool-miner-aleo-v1.0.4.3.tar.gz
(4)
8、修复batch参数设置无效，win10系统，如果算力低，可以尝试将batch设置32或者是64尝试下
(5)
9、修复跑段时间后，可能掉贡献的问题

如果不能正常运行，有下面2种可能
1、没安装VC运行环境(windows)
2、显卡驱动或者是CUDA没安装
https://developer.nvidia.com/cuda-11-7-0-download-archive
显示详细信息：
log
level: debug
(如果提示找不到 VCRUNTIME14，请下载安装vc_redist.x64.exe VC运行环境)

关于代理配置：
一个局域网内，代理只需要开一台就可以了，建议超过1台Miner的用户使用代理，在代理中有管理Miner相关信息
x-proxy使用步骤：
1、选择一个配置相对高的电脑，运行x-proxy
2、找到x-proxy的局域网IP,例如：192.168.1.88
3、在其它Miner机器上配置proxy: "http://192.168.1.88:9190/"
4、检查Miner的任务是不是每20s更新一次
