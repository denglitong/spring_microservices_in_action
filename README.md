# spring_mircroservices_in_action

Spring Microservices In Action.

![](./resources/P-1-14.png)

1. 核心微服务开发模式

        解决构建微服务的基础问题

    - 服务粒度
    - 通信协议
    - 接口设计
    - 服务的配置管理
    - 服务之间的事件处理

        ![](./resources/P-1-08.png)

2. 微服务路由模式

        如何将客户的服务请求发送到服务的特定实例？
    
    - 服务发现
    - 服务路由

        ![](./resources/P-1-09.png)

3. 微服务客户端弹性模式

        防止单个服务（或服务实例）中的问题级联暴露给服务的消费者

    - 客户端负载均衡
    - 断路器模式（确保客户端不会重复调用出现故障的服务）
    - 后备模式（在客户端失败时，客户端能否采用另一种方法来采取行动）
    - 舱璧模式（如何在客户端上隔离不同的服务调用，以确保表现不佳的服务不占用客户端上的所有资源）

        ![](./resources/P-1-10.png)

4. 微服务安全模式

    - 验证（如何确定调用服务的客户端就是它们声称的那个主体）
    - 授权（如何确定调用微服务的客户端是否允许执行它们正在进行的操作）
    - 凭据管理和传播（如何避免客户端每次都要提供凭据信息才能访问事务中涉及的服务调用）

        ![](./resources/P-1-11.png)

5. 微服务日志记录和跟踪模式

        微服务的缺点是调式和跟踪应用程序和服务中发生的事情要困难得多
        
    - 日志关联（一个用户事务会调用多个服务，如何将这些服务所生成的日志关联到一起？）
    - 日志聚合（如何将微服务生成的所有日志合并到一个可查询的数据库中）
    - 微服务跟踪（如何在涉及的所有服务中可视化客户端事务的流程，并了解其性能特征）

        ![](./resources/P-1-12.png)

6. 微服务构建和部署模式

    - 构建和部署管道（如何创建一个可重复的构建和部署过程，只需一键即可构建部署到任何环境）
    - 基础设施即代码（如何将服务的基础设施作为可以在源代码管理下的代码去对待）
    - 不可变服务器（一旦创建了微服务镜像，如何确保它在部署之后永远不会更改）
    - 凤凰服务器（配置漂移问题：如何确保运行微服务的服务器定期被拆卸，并重新创建一个不可变的镜像）

        ![](./resources/P-1-13.png)

