# gxgk-wechat-server
莞香广科微信公众号后端，为在校学生提供一系列信息查询与便民服务。

!["微信号 GXGKBBS"](http://77g5h8.com1.z0.glb.clouddn.com/qrcode.jpg)

功能介绍：

- 成绩查询
- 天气查询
- 常用电话
- 客服留言
- 气象雷达
- 公交路线
- 校历查询
- 学校新闻
- 合作信息
- 机器人陪聊
- 签到排行榜
- 明信片查询
- 随机音乐播放
- 校内图书馆搜索
- 四六级成绩查询
- HTML5 小游戏
- 广科微信社区入口
- 莞香广科论坛入口
- 上网认证客户端引导下载
- 快递查询、快递动态提醒

安装

```
pip install -r requirements.txt
``` 

运行

```
python run.py
```

部署

```
# using gunicorn
pip install gunicorn

# run
gunicorn run:app -p wechat.pid -b 127.0.0.1:8000 -D

# reload
kill -HUP `cat wechat.pid`
```
