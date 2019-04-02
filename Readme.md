# 说明
pip install twine
## 功能
1. 作为公共的库供各功能模块使用

部署新版本

python setup.py sdist
twine upload dist/*



## Util
Util 是通用的中间库，主要功能如下：
* 用于对消息处理封装
* 读取配置文件封装
* 对OTS的操作处理封装
* 对mysql 的操作封装
* 手机号MD5的解密

## 文件说明
* decipheringapi.py --手机号解密，前期用现成接口，后续考虑更新为ots
* mqapi.py -- rabbitMQ 队列接口
* otsapi---tablestore接口
* sqlapi----mysql接口
* functionapi ----一些常用功能的封装，提高复用性