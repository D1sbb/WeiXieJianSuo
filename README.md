# WeiXieJianSuo
威胁检索工具，利用微步API检索本地进程。

夜班无聊看群里聊天有这个需求，就写了个工具，没啥技术含量，上机排查可以用用。

## 1.0.8
优化循环检索(添加循环清空选择框 不勾选可减少资源消耗)

增加白名单sha值

更换编译器

## 启动
<del>工具会远程访问一个文本</del>(为了减少工具报毒，只能写到内存里)，里面是已经调用过微步API检索过的sha256值。如果你的进程和sha256值匹配，列表框会自动过滤掉此进程。
![image-1](https://raw.githubusercontent.com/D1sbb/WeiXieJianSuo/main/assets/1.jpg)

## 快速检索
输入你要查的域名或者IP(编辑框什么都不填，则会查询所有进程的TCP连接)

即可检索进程是否进行TCP连接，可一直点点点。
![image-2](https://raw.githubusercontent.com/D1sbb/WeiXieJianSuo/main/assets/2.jpg)

## 深度扫描
勾选则无视工具自带的白名单sha256值

## 检索前清除TCP信息
勾选就清空编辑框里的日志，再输出内容

## 双击列表框某个进程
会调用微步API进行分析
![image-3](https://raw.githubusercontent.com/D1sbb/WeiXieJianSuo/main/assets/3.jpg)

## UDP
勾选就查UDP连接 好像没啥用

## 工具自带本人APIKEY，每天只能使用300次
你也可以替换成自己的APIKEY

找到工具运行目录，双击Disbb.ini配置文件修改

## 麻辣香锅木马重启后 查询域名
![image-5](https://raw.githubusercontent.com/D1sbb/WeiXieJianSuo/main/assets/5重启后.jpg)

## 需要什么功能，可以加
新增 数字签名
![image-5](https://raw.githubusercontent.com/D1sbb/WeiXieJianSuo/main/assets/6%E6%96%B0%E5%A2%9E%E8%8E%B7%E5%8F%96%E6%95%B0%E5%AD%97%E7%AD%BE%E5%90%8D.jpg)

新增 导出进程内存数据
![image-4](https://raw.githubusercontent.com/D1sbb/WeiXieJianSuo/main/assets/4%E8%BD%AC%E5%AD%98%E6%96%87%E4%BB%B6%E5%88%86%E6%9E%90%E6%81%B6%E6%84%8F%E5%9F%9F%E5%90%8D.jpg)
