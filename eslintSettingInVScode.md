## VScode ESlint 代码自动格式化
问题：  
Vue项目使用ESlint检查代码风格，报错过多  
解决方法：  
1. 在VScode添加ESlint、vetur插件
2. 修改VScode用户设置，如下:  
    //添加进用户设置  
    ```json
    {
      ...,
    "eslint.autoFixOnSave": true,
    "eslint.validate": [
        "javascript",
        {"language": "vue",
        "autoFix": true},
        "javascriptreact",
        "vue"
    ]}
    ```

参考：<https://www.jianshu.com/p/69bfcb95b8d7>, <https://cloud.tencent.com/developer/article/1018838>