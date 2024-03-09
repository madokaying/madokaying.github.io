# spring入门以及环境配置

这两天一直在配置spring，maven的环境，踩了不少坑，这里记录一下  
1. maven的版本要和自己的jdk版本匹配，且settings.xml内的配置一定要设置好且不能有错，比如仓库的设置，镜像网址的设置，这里最好选择阿里云的镜像，不用vpn也能下载的很快，其次是settings.xml内不能有语法错误。
2. 现在创建的spring默认都是3.x.x的版本，这些版本适配的只有Java17和21.这里我的Java还是11版本，因此要在创建完spring项目后在pom.xml内修改spring的版本和JavaVersion，我这里修改成了2.7.4（spring）和11（JavaVersion），别的依赖部分能不改就先不改，然后右上角点击maven的reload（我这里好像是reimport），然后等待下载即可
3. 我在实际配置环境的时候遇到了jar下载不完全以及点击reload完全没反应的情况，这种情况可以先重启idea，然后再继续试（这两天我用重启已经成功解决了两次问题，亲测有效）

目前spring项目已经能正常启动 By 14:54
