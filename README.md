# CustomORM

**自定义ORM实现：**

    ·通过java中的pojo模型完成数据库表的映射操作
    ·1.手动方式：string-->varchar ...等
    ·2.hibernate-->完整的ORM模型，操作的是对象==>自己优化
    ·3.mybatis-->伪ORM框架--实际上操作的还是数据库==>动态sql，自带sql优化
    ---------
    ·4.内部映射转换器，根据映射自己选择属性类
    ·5.引入注解JPA:
        `@Table--完成类和表名映射
        `@Entity-告诉ORM这是POJO
        `@Id-----标识主键
        `@Column-标识属性映射的字段名称
        `@ManyToOne
        `@ManyToMany
        `OneToOne
        
**ORM映射：**
    
    1.实体名称--类名称
    2.字段名称--属性名称
    3.字段类型--java中兼容的属性类型
    -------
    4.主要用到技术:模板模式+反射+接口

**ORM映射：--表！=类**

    主要技术：
        1.自定义注解---
        2.反射获取注解判断
     后期优化：
        1.连接池-线程安全
        2.工厂创建    

    

    

    
