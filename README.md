编程浪子pi3Robot控制系统
=================================
## QuickStart
* Python3
* pip install -r requirements.txt

## 启动
* 启动web服务
    * export ops_config="local|production" && python manage.py runserver
* 启动Job
    * export ops_config="local|production" && python manage.py runjob -m weather/index

## MiniPC
* [MiniPC部署](./docs/)

## 重要文档
* [重要文档](./docs/)

## ToDoList
* [snoboy离线唤醒，可以自定义关键词 例如 芝麻开门等等](https://github.com/Kitt-AI/snowboy)
* [控制 博联RM PRO](https://github.com/mjg59/python-broadlink)
* [TTS 和 STT 换成 讯飞](https://console.xfyun.cn/app/myapp?currPage=1&keyword=)
* [homeassistant](https://www.domoticz.cn/)
* [增加elasticsearch，自动抓取互联网上感兴趣的主题,例如新闻，科技，互联网](https://www.elastic.co/cn/products/elasticsearch)

## 代码目录结构
* [mvc](./docs/mvc.md)


## 相关文档
* [Flask参考文档](./docs/flask.md)
* [TensorFlow](http://www.tensorfly.cn/)
* [树莓派上搭建唤醒词检测引擎 Snowboy](https://www.cnblogs.com/rnckty/p/8067115.html)
* [叮当](https://github.com/wzpan/dingdang-robot)
* [HomeAssistant文档](https://www.hachina.io/docs/321.html)
* [科大讯飞语音识别和合成](http://doc.xfyun.cn/rest_api/%E8%AF%AD%E9%9F%B3%E5%90%AC%E5%86%99.html)
* [broadlink](https://github.com/mjg59/python-broadlink)
* [DNSPOD]( https://www.dnspod.cn/docs/records.html#record-modify )
    * 可以通过API实现DDNS(动态dns解析)，通过脚本请求解析域名ip和外网ip是否一致
* [Ubuntu aria2](https://blog.csdn.net/crazycui/article/details/52205908)
    * https://aria2.github.io/
    * https://blog.icehoney.me/posts/2015-01-31-Aria2-download
* [you-get 获取视频地址](https://github.com/soimort/you-get)
* [python的webrtc库实现语音端点检测](https://www.jianshu.com/p/91f9f470f0f9)

## 问题处理
* 安装 MySQL-python ，结果出错 ImportError: No module named 'ConfigParser'

        在 Python 3.x 版本后，ConfigParser.py 已经更名为 configparser.py 所以出错！
        解决方法：pip install mysqlclient
