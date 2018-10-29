### Product

Product表示的就是系统中商品,它属于某个具体的类目节点和SKU 之间的关系是一对多的关系, Product 不能独立于SKU 单独存在, 其必须有一个default SKU ,如果一个Product 下面没有任何SKU 其将被删除

### SKU

SKU 是商品售卖和加入购物车的最小单位, 拥有价格信息,尺码以及颜色 等销售属性 , 是商品的具体表现形式

### Order

Order 是系统中大部分流程流转所需要处理的核心对象,从购物车checkout 开始,到付款,拆单,价格管理,物流管理等都需要使用到Order 和OrderService,主要由Distributor 生成

### Cart

Cart 表示的系统购物车, 用户可以将Sku 加入到购物车

### Distributor

Distributor 是系统中的分销商客户



### PurchaseOrder

采购单用于系统发送至VMS 的流转订单,通过Distributor 下单后,经订单拆单流程生成出来.



