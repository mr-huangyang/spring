##### 关键的几个类
* SpringManagedTransaction
* SqlSessionTemplate 
* SqlSessionUtils 创建sqlsession 并交给spring 管理
* SqlSessionFactoryBean 集成 spring 

``
spring 接管的大致流程 代理Mapper -> SqlSessionTemplate -> SqlSession[ Connection -> Transaction(mybatis) -> Executor -> SqlSession]
``