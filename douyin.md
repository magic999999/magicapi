
# 抖音接口

接口说明
* 账号注册请联系v:ping0206guo，添加好友请备注:api
* 所有接口均有权限验证，每个用户有唯一的token
* 所有接口均返回json格式，其中 code 为 0 时表示响应成功，
* 会增加调用次数。否则不会影响调用量。
* 所有接口响应都很快，timeout 时间建议在5s内
* 如需其他接口和数据，可定制开发
* 内部使用，侵权联系删除
* 所有接口没有特殊说明请求方式均为 GET


## 获取用户信息（app 字段丰富）
```
path：
/dy/user

params：	
token	    验证码   
user_id     用户id

response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```

## 获取用户信息（字段简单）
```
path：
/dy/user/v2

params：
token	    验证码
user_id     用户id

response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```

## 获取用户视频列表（app）
```
path：
/dy/user/video

params：
token	    验证码
user_id     用户id
page        翻页，默认为0，从0开始

response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```

## 获取用户视频列表（备用）
```
path：
/dy/user/video/v2

params：
token	    验证码
user_id     用户id
cursor      翻页，默认为0，上一次请求结果中max_cursor


response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```


## 获取视频评论
```
path：
/dy/comment

params：
token	     验证码
video_id     视频id
page         翻页，默认为0，从0开始


response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```

## 获取单个视频信息
```
path：
/dy/video/info

params：
token	     验证码
video_id     视频id
page         翻页，默认为0，从0开始


response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```

## 搜索用户列表
```
path：
/dy/search/user

params：
token	     验证码
keyword      关键词
page         翻页，默认为0，从0开始


response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```

## 搜索视频列表
```
path：
/dy/search/video

params：
token	     验证码
keyword      关键词
page         翻页，默认为0，从0开始


response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```

## 搜索视频列表（PC）
```
path：
/dy/search/video/pc

params：
token	     验证码
keyword      关键词
sort_type    # sort_type 2 最新发布 # sort_type 0 综合 # sort_type 1 综合


response：
返回值与抖音接口一样，对数据进行透传，请按照抖音页面对照理解意思
```