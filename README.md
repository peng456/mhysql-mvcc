# mhysql-mvcc
学习下，记录下。


mvcc  为什么存在？
因为需要，解决并发问题。
早期数据库，支持并发很弱，随着需求增长，并发越来越常见。并发的方案也就被不多发明出来。

早期数据库支持的并发只支持： 读读并发  ==》 but 读写、写读、写写  都需要 阻塞的===》 严重影响效率，并发太小
（https://segmentfault.com/a/1190000012650596）
==》 so mvcc 被提出来  ==》 不同数据库有不同的实现方式  1、Postgres  数据行上多版本 2、mysql 利用undolog 实现

mysql mvcc MVCC是行级锁的一个变种；实现方式大抵两种：悲观锁（pessimistic）、乐观锁（optimistic）

mysql 事务性存储  基于提升并发性能的考虑,



https://www.google.com/search?q=mysql+mvcc&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjsj7f63ZjjAhVGHc0KHS4BBOMQ_AUIECgB&biw=1920&bih=968


https://www.processon.com/view/5905e1aee4b0af9ce9b4d59e

https://blog.csdn.net/w2064004678/article/details/83012387
