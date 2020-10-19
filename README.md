# gotool

## 简介
Gotool是一个小而全的Go工具类库，通过静态方法封装，降低相关API的学习成本，提高工作效率，使Go拥有函数式语言般的优雅，让Go语言也可以“甜甜的”。

Gotool中的工具方法来自于每个用户的精雕细琢，它涵盖了Java开发底层代码中的方方面面，它既是大型项目开发中解决小问题的利器，也是小型项目中的效率担当；

Gotool是项目中“util”包友好的替代，它节省了开发人员对项目中公用类和公用工具方法的封装时间，使开发专注于业务，同时可以最大限度的避免封装不完善带来的bug。

### Gotool名称的由来

Gotool = Go + tool

### Gotool如何改变我们的coding方式

Gotool的目标是使用一个工具方法代替一段复杂代码，从而最大限度的避免“复制粘贴”代码的问题，彻底改变我们写代码的方式。

以计算MD5为例：

- 【以前】打开搜索引擎 -> 搜“Go MD5加密” -> 打开某篇博客-> 复制粘贴 -> 改改好用
- 【现在】引入Gotool -> SecureUtil.md5()

Gotool的存在就是为了减少代码搜索成本，避免网络上参差不齐的代码出现导致的bug。

-------------------------------------------------------------------------------

## 包含组件
一个Go基础工具类，对文件、流、加密解密、转码、正则、线程、XML等JDK方法进行封装，组成各种Util工具类，同时提供以下组件：

| 模块                |     介绍                                                                          |
| -------------------|---------------------------------------------------------------------------------- |
| Gotool-aop         |     JDK动态代理封装，提供非IOC下的切面支持                                              |
| Gotool-bloomFilter |     布隆过滤，提供一些Hash算法的布隆过滤                                                |
| Gotool-cache       |     简单缓存实现                                                                     |
| Gotool-core        |     核心，包括Bean操作、日期、各种Util等                                               |
| Gotool-cron        |     定时任务模块，提供类Crontab表达式的定时任务                                          |
| Gotool-crypto      |     加密解密模块，提供对称、非对称和摘要算法封装                                          |
| Gotool-db          |     JDBC封装后的数据操作，基于ActiveRecord思想                                         |
| Gotool-dfa         |     基于DFA模型的多关键字查找                                                         |
| Gotool-extra       |     扩展模块，对第三方封装（模板引擎、邮件、Servlet、二维码、Emoji、FTP、分词等）            |
| Gotool-http        |     基于HttpUrlConnection的Http客户端封装                                            |
| Gotool-log         |     自动识别日志实现的日志门面                                                         |
| Gotool-script      |     脚本执行封装，例如Javascript                                                     |
| Gotool-setting     |     功能更强大的Setting配置文件和Properties封装                                        |
| Gotool-system      |     系统参数调用封装（JVM信息等）                                                      |
| Gotool-json        |     JSON实现                                                                       |
| Gotool-captcha     |     图片验证码实现                                                                   |
| Gotool-poi         |     针对POI中Excel和Word的封装                                                       |
| Gotool-socket      |     基于Java的NIO和AIO的Socket封装          