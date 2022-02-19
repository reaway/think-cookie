# think-cookie

## 安装
```bash
composer require reaway/think-cookie
```

## 用法
```php
use Think\Component\Cookie\Facade\Cookie;

require __DIR__ . DIRECTORY_SEPARATOR . 'vendor' . DIRECTORY_SEPARATOR . 'autoload.php';

// 设置Cookie 有效期为3600秒
Cookie::set('name', 'value', 3600);

// 永久保存Cookie
Cookie::forever('name', 'value');

// 删除cookie
Cookie::delete('name');

// 读取某个cookie数据
Cookie::get('name');
// 获取全部cookie数据
Cookie::get();

// 助手函数
// 设置
cookie('name', 'value', 3600);

// 获取
echo cookie('name');

// 删除
cookie('name', null);
```

## 文档

详细参考 [Cookie](https://www.kancloud.cn/manual/thinkphp6_0/1037636)