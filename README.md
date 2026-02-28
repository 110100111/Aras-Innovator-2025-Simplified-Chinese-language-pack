若配置正确，登陆后界面应如下图所示：

![default](https://github.com/user-attachments/assets/f9fa3a68-a396-4720-8dfe-10f6ce619b81)

原文件来自Aras官网提供的简体中文语言包38V1（地址：https://aras.com/en/support/downloads/language-packs-hotfixes/language-packs/simplifiedchineselanguagepack）

配置步骤：

1.编辑SETUP-DEFAULTS.CMD
  
  根据Aras Innovator安装目录下InnovatorServerConfig.xml中DB-connection标签更改
  
  SET SERVER_URL、
  
  SET DATABASE_ID、
  
  SET INNOVATOR_LOGIN、
  
  SET INNOVATOR_PASSWORD、
  
  SET DB_SERVER、
  
  SET DATABASE_NAME、
  
  SET SQL_LOGIN与
  
  SET SQL_PASSWORD
  
  的值（若安装时非必要修改项均为默认设置，则大概率只需修改SET DB_SERVER和SET SQL_PASSWORD）；

2.复制必须文件

  将语言包下Innovator文件夹和OAuthServer文件夹复制到Aras Innovator安装目录下（默认安装地址应为：C:\Program Files (x86)\Aras\Innovator）；

3.运行.bat文件

  依次运行
  
  001-IMPORT-I18N-CHANGES.BAT，
  
  003-RESTART-WEB-SERVICE.BAT，
  
  004-IMPORT-CHINESE_SIMP.BAT；

4.检查日志文件

  打开语言包中logs文件夹，文件夹中应有2份日志文件，打开应均有success字样。

注：具体步骤语言包中000-README.TXT文件有详细描述，以上仅为简述。

免责声明：

1.本汉化文件（以下简称“本资源”）仅为方便用户交流与学习之用，由汉化爱好者制作，并非官方正式版本；

2.本汉化文件仅供学习、研究和交流使用，汉化者仅出于个人兴趣进行翻译和整合。原文件的一切权利归原作者所有。汉化者不对因使用本文件产生的任何法律问题承担责任。任何组织或个人不得将本资源用于商业目的或进行非法传播，否则一切后果自负；

3.本资源以Aras官方提供的语言包为基础，通过DeepSeek翻译，豆包校对，仅供用户测试语言效果、了解汉化技术及促进学习交流，请用户在下载后 24 小时内删除本资源；

4.由于使用本资源而引起的任何问题（包括但不限于系统崩溃、数据丢失、硬件损坏、法律纠纷等），汉化者及发布平台均不承担任何责任；

5.使用本资源即表示您已仔细阅读并完全同意本免责声明的全部条款。若您不同意其中任何条款，请立即停止使用并彻底删除本资源。

感谢您对汉化工作的支持，请尊重知识产权，共同维护良好的创作环境。


  
最后

不得不说中文包里是没有中文的，一个汉化折腾好久，怀疑是配置过程出错也没怀疑过官方提供的语言包根本没汉化，感谢写了这篇帖子 （https://juejin.cn/post/7267108796987080763） 的老哥指出问题出在哪。
