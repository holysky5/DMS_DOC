### Product

Product表示的就是系统中商品,它属于某个具体的类目节点和SKU 之间的关系是一对多的关系, Product 不能独立于SKU 单独存在, 其必须有一个default SKU ,如果一个Product 下面没有任何SKU 其将被删除

### SKU

SKU 是商品售卖和加入购物车的最小单位, 拥有价格信息,尺码以及颜色 等销售属性 , 是商品的具体表现形式

### Order

Order 是系统中大部分流程流转所需要处理的核心对象,从购物车checkout 开始,到付款,拆单,价格管理,物流管理等都需要使用到Order 和OrderService





