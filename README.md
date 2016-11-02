### 作用是把你现有的数据库表结构和数据选择性导出生成yii2的迁移文件

1.下载模块源码解压缩到 `backend/modules/`

2.在 `backend/config/main.php` 添加如下配置
````
'modules' => [
        'migration' => [
            'class' => 'migration\Module',
        ]
    ],
'aliases' => [
        '@migration' => '@backend/modules/migration',
    ],
```
3.在你的后台访问 http://yourdomain/migration