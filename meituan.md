
# 美团商超接口

接口说明
* 账号注册请联系v:ping0206guo，添加好友请备注:api
* 所有接口均有权限验证，每个用户有唯一的token
* 所有接口均返回json格式，其中 code 为 0 时表示响应成功，
* 会增加调用次数。否则不会影响调用量。
* 所有接口响应都很快，timeout 时间建议在5s内
* 如需其他接口和数据，可定制开发
* 内部使用，侵权联系删除
* 所有接口没有特殊说明请求方式均为 GET


## 获取店铺详情信息
```
path：
/mt/shop/info

params：	
token	验证码   
shop_id	店铺id

response：
返回值与美团接口一样，对数据进行透传，请按照美团页面对照理解意思
```

## 获取店铺商品列表
```
path：
/mt/shop/items

params：
shop_id	  店铺id
cate_id	  分类id 详情里面的 data.food_spu_tags.tag
page	  翻页默认为0，从0开始
token     验证码

response：
返回值与美团接口一样，对数据进行透传，请按照美团页面对照理解意思
```

## 按照经纬度获取周边店铺
```
path：
/mt/poi/lng/lat/

params：
lng     经纬度
lat     经纬度
order	0 综合 5 最近
token   验证码

response：
返回值与美团接口一样，对数据进行透传，请按照美团页面对照理解意思
```
