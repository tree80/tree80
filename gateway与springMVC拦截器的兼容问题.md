不兼容的原因:

请求处理流程不同：Gateway 处理的是代理请求，不会进入Spring MVC的DispatcherServlet

上下文环境不同：Gateway 运行在Netty/WebFlux环境下，而MVC拦截器运行在Servlet环境下

编程模型不同：Gateway 基于Reactive编程，MVC基于阻塞式编程
