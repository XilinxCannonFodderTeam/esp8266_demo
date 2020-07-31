# 项目介绍
次数实现的是一个基于micropython的，使用esp8266，利用WiFi热点的形式，进行设备发现的demo

+ esp8266.py:此文件实现了esp8266开启WiFi热点，等待app发送特定报文，并对报文进行解析，通过magic_number来确认是否是正确的app，然后连接app发送的热点名称，通过此热点利用MQTT向服务器发送验证信息，并等待服务器回传的验证信息
+ simple.py:此文件为开源的MQTT的实现