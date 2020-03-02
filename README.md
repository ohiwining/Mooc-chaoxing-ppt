文件用于爬取日新学堂任务点中的ppt图片，并将图片添加到word文档中再发送至邮箱，通过邮箱可在任何设备上查看。

环境要求：
python 装有requests,python-docx包  可直接通过pip安装   除此之外py代码根目录新建一个名为PPTPIC的文件夹，用于存放ppt图片

源码配置：
PAGES = 53  ppt图片一共有多少页，直接通过ppt源网页查看
Sender = "xxxx@163.com"  # 发邮件的地址，目前只支持网易163邮箱
passwd = "xxxx"  # 发送者邮件的授权密码，网易163邮箱设置中打开smtp服务之后会提示设置密码
SendTo = "xxxx@qq.com" #目标邮箱  任意邮箱都可以
FirstPngUrl='''https://s3.ananas.chaoxing.com/doc/8d/32/59/a91d2205bb1400a3696c19763014d3e7/thumb/1.png'''#网页上第一个ppt图片的链接（一定要第一个！！！）
