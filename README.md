# AiChat-GPT-WEB
无论是个人还是企业，打造一款属于自己的稳定人工智能AI聊天系统是有必要的，AiChat机器人对话系统，时下火爆的一款AI聊天系统源码，相比其它ChatGPT镜像站，这款AiChat搭建更简单，成本更低！
![微信图片_20231029113644](https://github.com/YangZong934/AiChat-GPT-WEB/assets/145942471/9c9c98fd-aa0d-4fdb-bc47-f56780dab971)
![微信截图_20231029113540](https://github.com/YangZong934/AiChat-GPT-WEB/assets/145942471/d0322de7-94bb-4efb-87ff-6e086fdc97af)
![微信截图_20231029113723](https://github.com/YangZong934/AiChat-GPT-WEB/assets/145942471/0fbe0ac5-a881-4b06-9b95-157818be2189)

AiChat-GPT-WEB系统功能：

1.支持GPT3.5与GPT-4全模型！！！

2.支持新建对话：新建对话支持改名字支持置顶支持删除。

3.支持深色模式，白天黑夜切换。

4.支持一键清空全部新建对话缓存。

5.支持用户头像显示：通过获取QQ头像来设定网站用户头像，QQ头像与网站同步。

6.支持GPT模型指定：全模型后台指定，前台支持切换模型，支持头像区分模型。

7.支持GPT角色扮演，GPT可充当任何角色来满足用户的需求。

8.支持上下文连续对话，AI回答途中可以随时打断。

9.支持聊天界面一键回到底部，聊天记录再多也不用担心会到底部麻烦的问题。

10.支持用户邀请好友获取聊天对话次数，具体获取的次数站长后台设定。

11.支持联系客服显示，再也不用担心用户流失问题。

12.支持全局面具词：询问3.5模型3.5会回答自己是3.5而不是3哦，4.0模型会回答自己是4.0也不是3了。

13.支持前台自定义提示词，在后台一键修改即可。

14.支持用户个人中心，可修改密码与绑定邮箱。

15.支持显示会员信息，支持会员套餐购买，支持对话剩余次数查询。

16.支持第三方易支付与官方微信、支付宝。

17.支持GPT3.5模型与4.0模型不同套餐，单独购买，套餐不会混用。

18.支持回台自定义转发API，支持用户公告显示。

19.支持对接第三方发卡网，支持用户卡密开通会员套餐。

20.支持用户购买订单查询，支持***地区查支付比例。

搭建准备工作：

1.一台服务器安装宝塔面板

2.一个域名（服务器是国内的就需要备案域名，国外的服务器域名无需备案）

3.环境要求MYSQL版本5.7 PHP版本7.4以上包含7.4

4.ChatGPT的API，自行准备

AiChat-GPT-WEB搭建教程：

一、文件部署

安装步骤：

1.先将程序解压到服务器（安装源码看附件）。

2.新建一个数据库，确保数据库编码uft8mb4，导入AiChat机器人数据库，修改数据库编码格式请看最后面。

3.找到common目录进入，找到config.php文件进入修改新建的数据库账号密码即可。

二、扩展部署

扩展hunter.so（附件源码里有一份）

找到以下这个目录。放入这个hunter.so 文件

/www/server/php/74/lib/php/extensions/no-debug-non-zts-20190902

[no-debug-non-zts-20190902] 根据自己的情况 把hunter.so 放到这个目录下，重启74 php 环境

最后找到php设置安装图片设置配置一下即可

extension = /www/server/php/74/lib/php/extensions/no-debug-non-zts-20190902/hunter.so
![微信截图_20231031200044](https://github.com/YangZong934/AiChat-GPT-WEB/assets/145942471/9a82b30a-4b41-4f98-b82a-56628f74383a)

MYSQL版本5.7 PHP版本7.4以上包含7.4

请在mysqdl配置修改里面 mysqld开头下面加上两行：

character-set-server=utf8mb4

collation-server=utf8mb4_unicode_ci

然后保存重启MYSQL服务即可
![微信截图_20231031200144](https://github.com/YangZong934/AiChat-GPT-WEB/assets/145942471/050b1e6b-cf5c-4b88-a2e8-d4e515f0d197)

重启后正常，即可部署成功。

三、后台登陆

后台路径你的域名后面加上/admin

后台账号admin

后台密码123456

