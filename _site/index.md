## Welcome to ShaoLuBin Page

###安装依赖包
######命令行方式安依赖包 -vvv 看安装详情 :～3.1 指定版本安装
1. 编辑 composer.josn && composer update
2. composer require overtrue/wechat
3. composer require overtrue/wechat:~3.1

######更新全部
composer update -vvv
######更新指定包
composer update overtrue/wechat -vvv

###语义话版本号
*	MAJOR.MINOR.PATCH
	*	MAJOR: 通常会发生API变更，不向后兼容
	*	MINOR: 新增功能，但是向后兼容
	* 	PATCH: 补丁，向后兼容，修复 bug.

###Release Operators(使用版本号)
*	"~": 指定向后兼容的最小版本
	* 	～1.2 等于 >= 1.2 && < 2.0.0
	*  ~1.2.3 等于 >= 1.2.3 && < 1.3.0

*	"^": 允许大版本前的所有版本
	* 	～1.2 等于 >= 1.2 && < 2.0.0
	*  ~1.2.3 等于 >= 1.2.3 && < 2.0(区别在这里)
	
*	确定版本：1.0.2

###版本锁定
*	版本锁定文件：composer.lock
*	composer install 产生它 & 使用它
*  composer update 更新它
*  composer.lock 是否应该加入版本控制？YES

###自动加载
```
“autoload”:{
	"psr-4" : {"Converter\\":"src/"}
}
```

###包的发布 lesson1.mp4 48:00

###参考资料
*	http://packagist.org/
*  http://getcomposer.org/
*  http://www.php-fig.org/
*  http://semver.org/
*  http://www.phpcomposer.com/

####安装laravel
注意事项:

Application Key is success
应用加密Key  php artisan key:generate

1. chmod -R 777 storage/        日志文件夹权限,线上不可用777
2. chmod -R 777 bootstrap/cache 缓存文件夹

####目录结构
http://d.laravel-china.org/docs/5.3/structure

可执行命令
chmod +x test
