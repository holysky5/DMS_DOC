### 系统的拓扑图结构如下

![](/assets/logic_arch.png)

#### 1. 客户端层

Web 层主要包括用户通过Internet 到达网关这一层,具体方式为B端客户使用 小程序,手机 H5 或者浏览器 访问公司服,其中 需要的技术和机器结构为 CDN\(提供图片和部分URL 的加速服务\) Gateway 公司内采用Nginx

#### 2. API 层

API 层职责主要是顶层Controller, 负责校验参数,路由具体服务,组合Service 层和第三方系统Wrapper 的返回值.以及特定应用的接口主要包含四个部分

1. H5 Server \(H5 server 可以采用mpvue 等 能直接编译成h5 和小程序的复用框架\) H5 或官网站点
2. Admin Server 管理类目,产品,价格,等Admin 后台
3. API 层 负责与其他系统的交互. 
4. Batch 提供系统所有的批处理任务

#### 3. Service层

Service 层是独立部署的业务逻辑执行层, 主要包含商品,订单,类目等实体的管理,以及第三方系统\(cms,wms,oms,vms\)返回值错误封装

### 4. 存储层

存储层提供了系统的数据存储\(mongo\),客户端登录用户追踪,缓存处理\(redis\),搜索服务\(solr\)等处理dao 功能.



### 系统框架选择





