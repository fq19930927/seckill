# seckill
java高并发秒杀api
Mysql:事务+行级锁

MySQL 5.5版本需要把create_time字段放在start_time和end_time前面 

dao层工作演变为:接口设计+sql编写

当抛出运行期异常时,声明式事务会回滚

cdn(内容分发网络):加速用户获取数据的系统,部署在离用户最近的网络节点上,命中cdn后不需要访问后端服务器

//优化思路:把客户端逻辑放到mysql服务端,避免网络延迟和GC影响

//两种解决方案
1.定制sql方案,update/*+[auto_commit]*/需要修改sql源码
2.使用存储过程,整个事务在mysql端完成
