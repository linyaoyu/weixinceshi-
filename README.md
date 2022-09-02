# daily_reminder
给女朋友做的微信天气推送

教程链接

https://www.coolapk.com/feed/38579891?shareKey=NGI3ZGZlZTM4MDBjNjMwMzdlM2M~&shareUid=3198334&shareFrom=com.coolapk.app_4.10




网址1   http://mp.weixin.qq.com/debug/cgi-bin/sandboxinfo?action=showinfo&t=sandbox/index
网址2   https://id.qweather.com/


模板内容如下：

{{date.DATA}} 

地区：{{region.DATA}} 

天气：{{weather.DATA}} 

气温：{{temp.DATA}} 

风向：{{wind_dir.DATA}} 

今天是我们恋爱的第{{love_day.DATA}}天 

{{birthday1.DATA}} 
{{birthday2.DATA}}


{{note_en.DATA}} 
{{note_ch.DATA}}


天气key生成教程
![image](https://raw.githubusercontent.com/limoest/daily_reminder/main/%E5%92%8C%E9%A3%8E%E5%A4%A9%E6%B0%94key%E7%94%9F%E6%88%90.png)


可以去天行数据申请各种各样的接口用来推送  
![image](https://raw.githubusercontent.com/limoest/daily_reminder/main/others/Snipaste_2022-08-24_12-13-19.png)
![image](https://raw.githubusercontent.com/limoest/daily_reminder/main/others/Snipaste.png)



有别的建议欢迎留言


{
# 公众号配置
# 公众号appId
"app_id": "wx63738c674f36bb06",
# 公众号appSecret
"app_secret": "22ec5a1bfb77abfbc46ac812de44872c",
# 模板消息id
"template_id": "K-65FRTwV7WfCHxE-eriQYCzlm6xaetlR7TBuedowhs",
# 接收公众号消息的微信号，如果有多个，需要在[]里用英文逗号间隔，例如["wx1", "wx2"]
"user": ["oHnJU6Bh_F4h8CyYsjBsSNnPsq80"],
 
# 信息配置
# 和风天气apikey
"weather_key": "0f2581914a454973b5072632d61185a6",
# 所在地区，可为省，城市，区，县，同时支持国外城市，例如伦敦
"region": "郑州市",
# 生日1，修改名字为对应需要显示的名字，如果生日为农历，在最前面加上r即可
"birthday1": {"name": "乖", "birthday": "2001-01-01"},
# 生日2
"birthday2": {"name": "乖", "birthday": "2002-01-01"},
# 在一起的日子，格式同上，暂不不支持农历
"love_date": "2022-01-01",
# 金句中文，如果设置了，则会显示这里的，如果为空，默认会读取金山的每日金句
"note_ch": "",
# 金句英文
"note_en": ""
}
