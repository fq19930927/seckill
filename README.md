# seckill
java高并发秒杀api
Mysql:事务+行级锁

MySQL 5.5版本需要把create_time字段放在start_time和end_time前面 

dao层工作演变为:接口设计+sql编写

当抛出运行期异常时,声明式事务会回滚
