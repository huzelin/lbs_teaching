LBS服务端口与branch分配
-----------
```
学生姓名   用户名  端口号          svn路径
 全为上     st1    10001    svn://127.0.0.1/repo/dev/branches/st1
 余少俊     st2    10002    svn://127.0.0.1/repo/dev/branches/st2
 汤晟皓     st3    10003    svn://127.0.0.1/repo/dev/branches/st3
 秦浚博     st4    10004    svn://127.0.0.1/repo/dev/branches/st4
 徐立       st5    10005    svn://127.0.0.1/repo/dev/branches/st5
 段文静     st6    10006    svn://127.0.0.1/repo/dev/branches/st6
 马梵博为   st7    10007    svn://127.0.0.1/repo/dev/branches/st7
```

整体服务架构
----------------
![](https://github.com/huzelin/lbs_teaching/blob/master/resource/arch.png) 

* 出租车模拟器
```
启动：
 $ cd mod/bin/simulator
 $ ./start.sh
关闭：
 $ ./stop.sh
```

* LBS服务程序
```
启动:
 $ cd mod/bin/mod-server
 $ ./run.sh
关闭：
 $ ./stop.sh
```

* UI界面
```
Android客户端：
   $ https://github.com/huzelin/lbs_teaching/android

http请求:
 范围查询：
   $ curl http://123.57.237.171:10001?query=range&range=106.1,107.1,39.9,39.9
 最近邻查询：
   $ curl http://123.57.237.171:10001?query=nn&pos=106.1,39.9
 结果为Json格式
```

