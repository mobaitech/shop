# shop(doing)
`注：` 该项目由vue构建框架,鉴于这不是最主要考察前端以及相关技术不熟练或未掌握(比如路由实现局部刷新（懒加载）vue-router），就不把前端写复杂了，尽量展示API调用接口实现数据库的功能

## 登录界面:

登录页面形式如下：

![image-20240529111028114](./images/image-20240601180454600.png)

页面实现代码见components下login文件夹的login.vue文件，主要是用fetch调用后端API接口：这里不再赘述。

后端再通过数据库查询实现，通过返回信息（200，500等状态码实现登录判断）再通过前端反馈信息实现下列功能

### 登录功能:

#### 登录密码错误信息显示:

通过alert警告框实现

![image-20240529111050259](./images/image-20240601180513196.png)

#### 输入密码警告框:

![image-20240529111106123](./images/image-20240601180532920.png)

#### 正确登录:

正确登录会跳出加载动画，动画结束后进入index主页

![image-20240529111124087](./images/image-20240601180612213.png)

#### 允许跳过登录:

> 但是跳过登录很多功能都无法使用

![image-20240529111203098](./images/image-20240601180624044.png)

### 忘记密码界面:

> 暂不支持改密功能：需要改密请练习管理员

![image-20240529111429728](./images/image-20240601181621073.png)

### 注册功能:

> 调用接口注册用户

![adduser](./images/image-20240601181634343.png)

#### 注册信息提示:

> 用户名是必填项：密码不一致也有提示信息

![image-20240529111613168](./images/image-20240601181646910.png)

两个弹窗警告：

![image-20240529111642904](./images/image-20240601181705563.png)

![image-20240529111651622](./images/image-20240601181719992.png)

> 这里注册一个mobaisilent用于演示

#### 注册成功

![image-20240529111757320](./images/image-20240601181742337.png)

## 主页:

### 预览

#### 主页预览(上部）：

![image-20240529111904885](./images/image-20240601181757406.png)

#### 主页预览（下部）：

![image-20240529111930278](./images/image-20240601181808923.png)

### 功能区块

#### 双开门动画演示

![image-20240529112120164](./images/image-20240601181819209.png)



### 鼠标指针放入某个商品区域块实现”添加到购物车“按钮自动浮现:

![addbuton](./images/image-20240601181827693.png)

### 悬浮按钮与图片自动缩放

![image-20240529112213516](./images/image-20240601181837565.png)

### 点击图片实现图片单独展示

![image-20240601182031910](./images/image-20240601182031910.png)

### 动态文字与导航与侵权免责声明

![image-20240529112237389](./images/image-20240601181845410.png)

### 一键置顶与暗黑模式按键:

![image-20240529112315138](./images/image-20240601181853962.png)

### 暗黑模式:

![image-20240529112342191](./images/image-20240601181907640.png)

### 一键置顶

> 详见项目网页：暂不演示

### 搜索功能:

![image-20240529112639428](./images/image-20240601181922953.png)

### 添加至购物车:

现在对这三件商品添加至购物车

![](./images/image-20240601181931563.png)

同步数据更新

![t1](./images/image-20240601181937947.png)

## 购物车:

对上面添加到购物车的商品的信息展示

![t2](https://img.nxtf.net/cdmTK0.png)

### 结算功能:

> 显示的地址是多个地址中的第一个：详情请见 “我的地址” 区块

![t3](https://img.nxtf.net/LzYuEp.png)


### 提示功能:


![tr](./images/image-20240601182118906.png)

### 微信支付:

> 点击已付款默认扣除余额：（请勿随意付款，谨防诈骗）

![t23](./images/image-20240601182136328.png)

### 支付宝付款:

![tfjj](./images/image-20240601182149752.png)

### 取消支付

> 点击取消支付自动跳转到订单界面

![image-20240601182234600](./images/image-20240601182234600.png)

### 已付款功能:

> 付款之后实现修改余额，提示反馈信息:反馈信息如下

#### 付款成功

![jfsdk](./images/image-20240601182402928.png)



#### 付款失败

![image-20240601182303508](./images/image-20240601182303508.png)

