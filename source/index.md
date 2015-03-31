---
title: API Reference

language_tabs:
  - shell

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='http://sunnyflute.com'>Powered by 计算机界大龄竹笛少年</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the Kittn API! You can use our API to access Kittn API endpoints, which can get information on various cats, kittens, and breeds in our database.

We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

This example API documentation page was created with [Slate](http://github.com/tripit/slate). Feel free to edit it and use it as a base for your own API's documentation.

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace `meowmeowmeow` with your personal API key.
</aside>

# 折扣App

## 获取首页幻灯


```shell
curl "http://open.qyer.com/lastminute/app_slide"
```

> The above command returns JSON structured like this:

```json
{
  status: 1,
  info: "",
  times: 0,
  data: [
    {
      type: "product",
      h1: "上海直飞毛里求斯8天5晚自由行",
      h2: "3月 4月 5月",
      price: "1999",
      href: "http://m.qyer.com/z/deal/9991/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105177482165?imageView2/2/w/310"
    },
    {
      type: "product",
      h1: "Beijing飞东京6天5晚自由行",
      h2: "4月 ",
      price: "7999",
      href: "http://m.qyer.com/z/deal/23840/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/10/08/14127635005094?imageView2/2/w/310"
    },
    {
      type: "product",
      h1: "北京直飞南极8天8晚自由行",
      h2: "3月 4月 6月 7月 8月 9月 10月 11月 12月",
      price: "98765",
      href: "http://m.qyer.com/z/deal/10121/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310"
    },
    {
      type: "campaign",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310",
      href: "http://m.qyer.com/weixin/score.php?campaign=apppromotion&category=h5top&source=app"
    }
  ]
}
```

This endpoint retrieves all data home page need.

### HTTP Request

`GET http://open.qyer.com/lastminute/app_slide`

### Query Parameters

`不需要参数`


<aside class="success">
Remember — 之前的参数是得传的, 例如: 
oauth_token=33e4fcb72b252089930b65b4187cbf34
&client_secret=44c86dbde623340b5e0a
&client_id=qyer_discount_ios
&track_app_version=1.6.3
&track_os=ios%25208.2
&app_installtime=1421109485
&track_app_channel=App%2520Store
&track_deviceid=8EF77D0C-5531-4CD9-8176-6EDC49FFEC03
&track_device_info=iPhone%25205(ChinaMobile,ChinaTelecom,ChinaUnicom)
&track_user_id=5443973
&size=640x1136
</aside>




## 获取首页产品分类


```shell
curl "http://open.qyer.com/lastminute/app_productType"
```

> The above command returns JSON structured like this:

```json
{
  status: 1,
  info: "success",
  times: 0,
  data: [
    {
      name: "自由行",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c9210409.png",
      type: "label"
    },
    {
      name: "机票",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c900b00d.png",
      type: "label"
    },
    {
      name: "酒店",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c8c84a56.png",
      type: "label"
    },
    {
      name: "签证",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c8a4fbfd.png",
      type: "label"
    },
    {
      name: "更多",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c887b847.png",
      type: "more"
    }
  ]
}
```

This endpoint retrieves all data home page need.

### HTTP Request

`GET http://open.qyer.com/lastminute/app_productType`

### Query Parameters

`不需要参数`


<aside class="success">
Remember — 之前的参数是得传的, 例如: 
oauth_token=33e4fcb72b252089930b65b4187cbf34
&client_secret=44c86dbde623340b5e0a
&client_id=qyer_discount_ios
&track_app_version=1.6.3
&track_os=ios%25208.2
&app_installtime=1421109485
&track_app_channel=App%2520Store
&track_deviceid=8EF77D0C-5531-4CD9-8176-6EDC49FFEC03
&track_device_info=iPhone%25205(ChinaMobile,ChinaTelecom,ChinaUnicom)
&track_user_id=5443973
&size=640x1136
</aside>


## 获取专题-可用于首页


```shell
curl "http://open.qyer.com/lastminute/app_popCampaign"
```

> The above command returns JSON structured like this:

```json
{
  status: 1,
  info: "",
  times: 0,
  data: [
    {
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2fb20d7.png",
      href: "http://m.qyer.com/z/deal/10057/?source=app"
    },
    {
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2d8f274.png",
      href: "http://m.qyer.com/z/deal/9993/?source=app"
    },
    {
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2b8dd92.png",
      href: "http://m.qyer.com/z/deal/9865/?source=app"
    }
  ]
}
```

This endpoint retrieves all data home page need.

### HTTP Request

`GET http://open.qyer.com/lastminute/app_popCampaign?page=<page>&pageSize=<pageSize>`

### Query Parameters

`不需要参数`


<aside class="success">
Remember — 之前的参数是得传的, 例如: 
oauth_token=33e4fcb72b252089930b65b4187cbf34
&client_secret=44c86dbde623340b5e0a
&client_id=qyer_discount_ios
&track_app_version=1.6.3
&track_os=ios%25208.2
&app_installtime=1421109485
&track_app_channel=App%2520Store
&track_deviceid=8EF77D0C-5531-4CD9-8176-6EDC49FFEC03
&track_device_info=iPhone%25205(ChinaMobile,ChinaTelecom,ChinaUnicom)
&track_user_id=5443973
&size=640x1136
</aside>



## 获取精选商品-可用于首页


```shell
curl "http://open.qyer.com/lastminute/app_selectedProduct?page=1&pageSize=10"
```

> The above command returns JSON structured like this:

```json
{
  status: 1,
  info: "",
  times: 0,
  data: [
    {
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2fb20d7.png",
      href: "http://m.qyer.com/z/deal/10057/?source=app"
    },
    {
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2d8f274.png",
      href: "http://m.qyer.com/z/deal/9993/?source=app"
    },
    {
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2b8dd92.png",
      href: "http://m.qyer.com/z/deal/9865/?source=app"
    }
  ]
}
```

This endpoint retrieves all data home page need.

### HTTP Request

`GET http://open.qyer.com/lastminute/app_popCampaign`

### Query Parameters

参数|类型| 必须|默认|描述 
--------- |--------- | --------- | ------- | -----------
page |int| 否 | 1 | 展示第几页数据 
pageSize|int| 否| 10 | 每页展示多少条数据



<aside class="success">
Remember — 之前的参数是得传的, 例如: 
oauth_token=33e4fcb72b252089930b65b4187cbf34
&client_secret=44c86dbde623340b5e0a
&client_id=qyer_discount_ios
&track_app_version=1.6.3
&track_os=ios%25208.2
&app_installtime=1421109485
&track_app_channel=App%2520Store
&track_deviceid=8EF77D0C-5531-4CD9-8176-6EDC49FFEC03
&track_device_info=iPhone%25205(ChinaMobile,ChinaTelecom,ChinaUnicom)
&track_user_id=5443973
&size=640x1136
</aside>



## 发现页混排列表


```shell
curl "http://open.qyer.com/lastminute/app_discover?page=1&pageSize=10"
```

> The above command returns JSON structured like this:

```json
{
  status: 1,
  info: "",
  times: 0,
  data: [
    {
      type: "product",
      h1: "0上海直飞毛里求斯8天5晚自由行",
      productType: "ziyouxing",
      h2: "3月 4月 5月",
      price: "1999",
      href: "http://m.qyer.com/z/deal/9991/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105177482165?imageView2/2/w/310"
    },
    {
      type: "product",
      h1: "1Beijing飞东京6天5晚酒店",
      productType: "jiudian",
      h2: "4月 ",
      price: "7999",
      href: "http://m.qyer.com/z/deal/23840/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/10/08/14127635005094?imageView2/2/w/310"
    },
    {
      type: "product",
      h1: "2北京直飞南极8天8晚签证",
      productType: "qianzheng",
      h2: "3月 4月 6月 7月 8月 9月 10月 11月 12月",
      price: "98765",
      href: "http://m.qyer.com/z/deal/10121/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310"
    },
    {
      type: "campaign",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310",
      href: "http://m.qyer.com/weixin/score.php?campaign=apppromotion&category=h5top&source=app"
    },
    {
      type: "product",
      h1: "4上海直飞毛里求斯8天5晚自由行",
      productType: "ziyouxing",
      h2: "3月 4月 5月",
      price: "1999",
      href: "http://m.qyer.com/z/deal/9991/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105177482165?imageView2/2/w/310"
    }
  ]
}
```

This endpoint retrieves all data home page need.

### HTTP Request

`GET http://open.qyer.com/lastminute/app_discover?page=<page>&pageSize=<pageSize>`

### Query Parameters

参数|类型| 必须|默认|描述 
--------- |--------- | --------- | ------- | -----------
page |int| 否 | 1 | 展示第几页数据 
pageSize|int| 否| 10 | 每页展示多少条数据



<aside class="notice">
为了展示美观, 样本返回数据只展示了不多的几条数据
</aside>
<aside class="success">
Remember — 之前的参数是得传的, 例如: 
oauth_token=33e4fcb72b252089930b65b4187cbf34
&client_secret=44c86dbde623340b5e0a
&client_id=qyer_discount_ios
&track_app_version=1.6.3
&track_os=ios%25208.2
&app_installtime=1421109485
&track_app_channel=App%2520Store
&track_deviceid=8EF77D0C-5531-4CD9-8176-6EDC49FFEC03
&track_device_info=iPhone%25205(ChinaMobile,ChinaTelecom,ChinaUnicom)
&track_user_id=5443973
&size=640x1136
</aside>

## Get a Specific Kitten


```shell
curl "http://open.qyer.com/lastminute/app_home"
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Isis",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">If you're not using an administrator API key, note that some kittens will return 403 Forbidden if they are hidden for admins only.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the cat to retrieve

参数| 默认|描述 
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

