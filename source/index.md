---
title: 穷游折扣-接口参考

language_tabs:
  - shell

toc_footers:
  - 疑问请联系 <a href="mailto:runxi.ding@qyer.com">丁润西</a> runxi.ding@qyer.com
  - Powered by 计算机界大龄竹笛少年

includes:

search: true
---

# 折扣App

## 获取幻灯,产品分类,热门专题-首页


```shell
curl "http://open.qyer.com/lastminute/app_home"
```

> The above command returns JSON structured like this:

```json
{
  status: 1,
  info: "",
  times: 0,
  data: {
    slide: [
      {
        id: 999,
        type: "deal",
        title: "上海直飞毛里求斯8天5晚自由行",
        departureTime: "3月 4月 5月",
        price: "<em>1074</em>元起",
        href: "http://m.qyer.com/z/deal/9991/?source=app",
        imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105177482165?imageView2/2/w/310"
      },
      {
        id: 23840,
        type: "deal",
        title: "Beijing飞东京6天5晚自由行",
        departureTime: "4月 ",
        price: "<em>10074</em>元起",
        href: "http://m.qyer.com/z/deal/23840/?source=app",
        imageUrl: "http://pic.qyer.com/public/picstock/2014/10/08/14127635005094?imageView2/2/w/310"
      },
      {
        id: 10121,
        type: "deal",
        title: "北京直飞南极8天8晚自由行",
        departureTime: "3月 4月 6月 7月 8月 9月 10月 11月 12月",
        price: "<em>98765</em>元起",
        href: "http://m.qyer.com/z/deal/10121/?source=app",
        imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310"
      },
      {
        id: 80,
        type: "topic",
        imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310",
        href: "http://m.qyer.com/z/zt/201503_03.html?source=app"
      }
    ],
    productType: [
      {
        id: 1018,
        catename: "自由行",
        imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c9210409.png"
      },
      {
        id: 1016,
        catename: "机票",
        imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c900b00d.png"
      },
      {
        id: 1017,
        catename: "酒店",
        imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c8c84a56.png"
      },
      {
        id: 1785,
        catename: "签证",
        imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4c8a4fbfd.png"
      }
    ],
    popTopic: [
      {
        id: 81,
        imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2fb20d7.png",
        href: "http://m.qyer.com/z/zt/201503_04.html?source=app"
      },
      {
        id: 70,
        imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2d8f274.png",
        href: "http://m.qyer.com/z/zt/201501_10.html?source=app"
      },
      {
        id: 73,
        imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a4f2b8dd92.png",
        href: "http://m.qyer.com/z/zt/201502_02.html?source=app"
      }
    ]
  }
}
```


### HTTP Request

`GET http://open.qyer.com/lastminute/app_home`

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
curl "http://open.qyer.com/lastminute/app_selected_product?page=1&pageSize=10"
```

> The above command returns JSON structured like this:

```json
{
  status: 1,
  info: "",
  times: 0,
  data: [
    {
      id: 10057,
      title: "上海直飞毛里求斯8天7晚酒店行(含各种签证各种费用)",
      departureTime: "3月 4月 5月",
      href: "http://m.qyer.com/z/deal/10057/?source=app",
      price: "<em>1074</em>元起",
      productType: "jiudian",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/3/31/551a51a3a2216.png"
    },
    {
      id: 9993,
      title: "上海直飞毛里求斯8天7晚机票行(含各种签证各种费用)",
      departureTime: "3月 4月 5月",
      href: "http://m.qyer.com/z/deal/9993/?source=app",
      price: "<em>8999</em>元起",
      productType: "feiji",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a51a602cfe.png"
    },
    {
      id: 9865,
      title: "上海/北京/香港直飞毛里求斯8天7晚自由行(含各种签证各种费用)",
      departureTime: "3月 4月 5月",
      href: "http://m.qyer.com/z/deal/9865/?source=app",
      price: "<em>99999</em>元起",
      productType: "ziyouxing",
      imgUrl: "http://test1362383214.qiniudn.com/lastminute/library/2015/03/31/551a51a808dd2.png"
    }
  ]
}
```


### HTTP Request

`GET http://open.qyer.com/lastminute/app_selected_product?page=<page>&pageSize=<pageSize>`

### Query Parameters

参数|类型| 必须|默认|描述 
--------- |--------- | --------- | ------- | -----------
page |Int 或 String| 否 | 1 | 展示第几页数据 
pageSize|Int 或 String| 否| 10 | 每页展示多少条数据



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



## 获取发现页混排列表


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
      id: 9991,
      type: "deal",
      title: "上海直飞毛里求斯8天5晚自由行",
      productType: "ziyouxing",
      departureTime: "3月 4月 5月",
      price: "<em>99999</em>元起",
      href: "http://m.qyer.com/z/deal/9991/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105177482165?imageView2/2/w/310"
    },
    {
      id: 23840,
      type: "deal",
      title: "Beijing飞东京6天5晚酒店",
      productType: "jiudian",
      departureTime: "4月 ",
      price: "<em>77779</em>元起",
      href: "http://m.qyer.com/z/deal/23840/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/10/08/14127635005094?imageView2/2/w/310"
    },
    {
      id: 10121,
      type: "deal",
      title: "北京直飞南极8天8晚签证",
      productType: "qianzheng",
      departureTime: "3月 4月 6月 7月 8月 9月 10月 11月 12月",
      price: "<em>7899</em>元起",
      href: "http://m.qyer.com/z/deal/10121/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310"
    },
    {
      id: 76,
      type: "topic",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105129438674?imageView2/2/w/310",
      href: "http://m.qyer.com/z/zt/201502_05.html?source=app"
    },
    {
      id: 9991,
      type: "deal",
      title: "上海直飞毛里求斯8天5晚自由行",
      productType: "ziyouxing",
      departureTime: "3月 4月 5月",
      price: "<em>99999</em>元起",
      href: "http://m.qyer.com/z/deal/9991/?source=app",
      imageUrl: "http://pic.qyer.com/public/picstock/2014/09/12/14105177482165?imageView2/2/w/310"
    }
  ]
}
```


### HTTP Request

`GET http://open.qyer.com/lastminute/app_discover?page=<page>&pageSize=<pageSize>`

### Query Parameters

参数|类型| 必须|默认|描述 
--------- |--------- | --------- | ------- | -----------
page |Int 或 String| 否 | 1 | 展示第几页数据 
pageSize|Int 或 String| 否| 10 | 每页展示多少条数据



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



## 获取分类页的分类


```shell
curl "http://open.qyer.com/lastminute/app_category"
```

> The above command returns JSON structured like this:

```json
{
    "status": 1,
    "info": "",
    "times": 0,
    "data": [
        {
            "id": 1016,
            "name": "fightTicket",
            "_comment": "机票"
        },
        {
            "id": 1017,
            "name": "hotel",
            "_comment": "酒店"
        },
        {
            "id": 1018,
            "name": "diyTour",
            "_comment": "自由行"
        },
        {
            "id": 1020,
            "name": "ship",
            "_comment": "邮轮"
        },
        {
            "id": 1785,
            "name": "visa",
            "_comment": "签证"
        },
        {
            "id": 1983,
            "name": "localTour",
            "_comment": "当地游"
        },
        {
            "id": 1049,
            "name": "insurance",
            "_comment": "保险"
        },
        {
            "id": 1021,
            "name": "carRental",
            "_comment": "租车"
        },
        {
            "id": 2161,
            "name": "euroTrainTicket",
            "_comment": "欧铁票"
        },
        {
            "id": 1050,
            "name": "ticketEtc",
            "_comment": "门票及其他"
        }
    ]
}
```


### HTTP Request

`GET http://open.qyer.com/lastminute/app_category`

### Query Parameters

`不需要参数`



<aside class="notice">
为了展示美观, 样本返回数据只展示了不多的几条数据
</aside>
<aside class="notice">
_comment字段中的数据仅仅是注释, 请勿使用
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


## 获取搜索热词


```shell
curl "http://open.qyer.com/lastminute/app_hot_searched_words"
```

> The above command returns JSON structured like this:

```json
{
    status: 1,
    info: "",
    times: 0,
    data: [
        "邮轮",
        "租车",
        "保险",
        "当地游",
        "欧铁票",
        "香港",
        "台湾",
        "泰国",
        "日本",
        "韩国",
        "新加坡",
        "马尔代夫",
        "澳大利亚"
    ]
}
```


### HTTP Request

`GET http://open.qyer.com/lastminute/app_hot_searched_words`

### Query Parameters

`不需要参数`




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





## 获取用户订单列表


```shell
curl "http://open.qyer.com/lastminute/app_get_userorderformlist?oauth_token=e458c75b658c5252c4c115ca737b2053&client_secret=44c86dbde623340b5e0a&client_id=qyer_discount_ios&track_app_version=1.6.3&is_show_supplier=1&is_show_pay=1&page=1&track_os=ios%25208.3&app_installtime=1421109485&track_app_channel=App%2520Store&track_deviceid=8EF77D0C-5531-4CD9-8176-6EDC49FFEC03&track_user_id=5287911&count=5&track_device_info=iPhone%25205(ChinaMobile,ChinaTelecom,ChinaUnicom)"
```

> The above command returns JSON structured like this:

```json
{
    status: 1,
    info: "",
    times: 0,
    data: {
        pager: "<div class="ui_page"><a data-bn-ipg="pages-3" href="javascript: orderlistpage(1)" class='ui_page_item ui_page_item_current'>1</a> <a data-bn-ipg="pages-3" href="javascript: orderlistpage(2)" class='ui_page_item'>2</a> <a data-bn-ipg="pages-5" href="javascript: orderlistpage(2)" class='ui_page_item ui_page_next' title="下一页">下一页</a> </div>",
        counts: "6",
        res: [
            {
                id: "1996795720",
                lid: "10207",
                pid: "1292",
                cid: "5836",
                sid: "1860",
                num: "1",
                name: "小美",
                phone: "18500192024",
                email: "sunnyding602@qq.com",
                uid: "5287911",
                unit_price: "0.01",
                price: "0.01",
                payment: "0",
                datetime: "1428547655",
                firstpay: "1",
                relid: null,
                buyer_email: null,
                buyer_id: null,
                notify_id: null,
                notify_time: null,
                notify_type: null,
                payment_type: null,
                seller_email: null,
                seller_id: null,
                sign: null,
                sign_type: null,
                total_fee: null,
                trade_no: null,
                trade_status: null,
                return_type: null,
                return_time: "",
                channel: "ios",
                guid: "",
                confirmstatus: "0",
                rooms: "0",
                msg: null,
                refund_status: null,
                refund_time: "0",
                refund_return_time: "0",
                refund_deal_time: "0",
                refund_reason: "",
                refund_verify_reason: "",
                refund_error: "",
                track_deviceid: "8EF77D0C-5531-4CD9-8176-6EDC49FFEC03",
                lastalipaydatetime: 1428547955,
                lastminute_title: "409秒杀LM",
                lastminute_price: "1000",
                products_type: 0,
                products_title: "1111",
                alipay_account: "raffi@126.com",
                supplier_title: "自己人",
                supplier_type: 0,
                supplier_phone: "15810922404",
                stock: 197,
                secondpay_start_time: 0,
                secondpay_end_time: 0,
                pay_type: 0,
                room_price_total: 0,
                products_departure_date: "2015/05/09",
                buyerinfo_name: "小美",
                buyerinfo_phone: "18500192024",
                buyerinfo_email: "sunnyding602@qq.com",
                lastminute: {
                    id: "10207",
                    title: "409秒杀LM",
                    product_type: "1785",
                    recommend: "0",
                    views: "19",
                    status: "0",
                    onsale: "1",
                    booktype: "1",
                    supplierid: "1860",
                    sort_time: "0",
                    sort_weight: "0",
                    pay_time: "1428544528",
                    start_time: "1428543682",
                    end_time: "1431619224",
                    travel_starttime: "1428508800",
                    travel_endtime: "1432828800",
                    abroad: "inland",
                    start_pos: "青岛",
                    continent: "a:1:{i:10;a:1:{i:0;s:2:"14";}}",
                    country: "英国",
                    city: "伦敦",
                    poi: "",
                    channel: "web,h5,mobile",
                    modifytime: "1428648572",
                    price: "1000",
                    list_price: "1000",
                    buy_price: "1",
                    feature: "",
                    pic: "http://test1362383214.qiniudn.com/public/lastmin/lastminute/2015/04/10/14286481337359",
                    timeout: "5",
                    soldnum: "0",
                    reservationday: "10",
                    use_if: "",
                    qyer_url: "",
                    url: "",
                    groupno: "",
                    travelday: "0",
                    travelnight: "0",
                    vehiclego: "0",
                    vehicleback: "0",
                    reservationtype: "1",
                    reservationdesc: "",
                    phone: "",
                    plan_id: "0",
                    discount_code: "",
                    order_type: "0",
                    login_visible: "0",
                    supplieradmin: "4632288",
                    adminid: "63",
                    role: "255",
                    end_pos: "英国,伦敦",
                    addtime: "1428543707",
                    modify: "189",
                    supplier: "1860",
                    isnew: "0",
                    start_date: "2015-04-09 09:41:22",
                    end_date: "2015-05-15 00:00:24",
                    pic_info: null,
                    reservationhour: "0",
                    reservationmin: "0",
                    offshelvestype: "1",
                    paymenttype: "1",
                    suppliermodify: "4632288",
                    verifystatus: "2",
                    soldout: "0",
                    csh: "["0571-87356978"]",
                    web_order: "0",
                    wsoldnum: "0",
                    weight: "0",
                    info_give: "",
                    detail_image: null,
                    booking_time: "2015年1月26日至12月31日",
                    travel_time: "",
                    ctn: "12",
                    op_pic: "",
                    op_pic1: "",
                    departure: "青岛",
                    relatid: "",
                    currency_code: "",
                    firstpay_start_time: "1428544528",
                    firstpay_end_time: "0",
                    secondpay_start_time: "0",
                    appoint_date: "0",
                    holiday: "",
                    relatepoi: "",
                    editadmin: "189"
                },
                supplier: {
                    id: "1860",
                    catename: "自己人",
                    catename_en: "test",
                    catename_py: "ceshi",
                    image: "http://test1362383214.qiniudn.com/public/lastmin/supplier/2014/05/30/1401448532",
                    sub_image: null,
                    alipay_account: "raffi@126.com",
                    phone: "15810922404",
                    siteurl: "http://www.qyer.com/",
                    email: "zidong.li@qyer.com",
                    type: "2",
                    status: "1",
                    uid: "5287890",
                    username: "putao888",
                    legal_person: "lilili",
                    full_catename: "呀1212121",
                    gid: "14",
                    show_user_info: "1",
                    submit: "0",
                    submittime: "0",
                    modify: "63",
                    modifytime: "1428384766",
                    royalty_status: "1",
                    complain_phone: "12345678",
                    emergency_phone: "400-1234567"
                },
                products: {
                    id: "1292",
                    lid: "10207",
                    sid: "1860",
                    title: "1111",
                    total: "0",
                    stock: "0",
                    price: "0.00",
                    advance_payment: "0.00",
                    buy_limit: "0"
                },
                orderform: {
                    id: "1996795720",
                    lid: "10207",
                    pid: "1292",
                    cid: "5836",
                    sid: "1860",
                    num: "1",
                    name: "小美",
                    phone: "18500192024",
                    email: "sunnyding602@qq.com",
                    uid: "5287911",
                    unit_price: "0.01",
                    price: "0.01",
                    payment: "0",
                    datetime: "1428547655",
                    firstpay: "1",
                    relid: null,
                    buyer_email: null,
                    buyer_id: null,
                    notify_id: null,
                    notify_time: null,
                    notify_type: null,
                    payment_type: null,
                    seller_email: null,
                    seller_id: null,
                    sign: null,
                    sign_type: null,
                    total_fee: null,
                    trade_no: null,
                    trade_status: null,
                    return_type: null,
                    return_time: null,
                    channel: "ios",
                    guid: "",
                    confirmstatus: "0",
                    rooms: "0",
                    msg: null,
                    refund_status: null,
                    refund_time: "0",
                    refund_return_time: "0",
                    refund_deal_time: "0",
                    refund_reason: "",
                    refund_verify_reason: "",
                    refund_error: "",
                    track_deviceid: "8EF77D0C-5531-4CD9-8176-6EDC49FFEC03"
                },
                qyer_des: "NTI4NzkxMWMyVnlkbWxqWlQwaWJXOWlhV3hsTG5ObFkzVnlhWFI1Y0dGNUxuQmhlU0ltWDJsdWNIVjBYMk5vWVhKelpYUTlJblYwWmkwNElpWnZkWFJmZEhKaFpHVmZibTg5SWxSWlJWSXhPVGsyTnprMU56SXdJaVp6ZFdKcVpXTjBQU0kwTURubnA1TG1uWUJNVFNJbWNHRjViV1Z1ZEY5MGVYQmxQU0l4SWlaelpXeHNaWEpmYVdROUluSmhabVpwUURFeU5pNWpiMjBpSm5SdmRHRnNYMlpsWlQwaU1DNHdNU0ltWW05a2VUMGlNVEV4TVNJbWJtOTBhV1o1WDNWeWJEMGlhSFIwY0NVelFTVXlSaVV5Um1Gd2FTNXhlV1Z5TG1OdmJTVXlSbTBsTWtaaGNIQmhiR2x3WVhsdWIzUnBabmt1Y0dod0lpWnBkRjlpWDNCaGVUMGlNakF4TlMwd05DMHdPU0F4TURvMU1qb3pOU0k9NDRjODZkYmRlNjIzMzQwYjVlMGE="
            },
            {
                id: "1996795662",
                lid: "10207",
                pid: "1292",
                cid: "5836",
                sid: "1860",
                num: "1",
                name: "小美",
                phone: "18500192000",
                email: "sunnyding602@qq.com",
                uid: "5287911",
                unit_price: "0.01",
                price: "0.01",
                payment: "0",
                datetime: "1428547478",
                firstpay: "1",
                relid: null,
                buyer_email: null,
                buyer_id: null,
                notify_id: null,
                notify_time: null,
                notify_type: null,
                payment_type: null,
                seller_email: null,
                seller_id: null,
                sign: null,
                sign_type: null,
                total_fee: null,
                trade_no: null,
                trade_status: null,
                return_type: null,
                return_time: "",
                channel: "ios",
                guid: "",
                confirmstatus: "0",
                rooms: "0",
                msg: null,
                refund_status: null,
                refund_time: "0",
                refund_return_time: "0",
                refund_deal_time: "0",
                refund_reason: "",
                refund_verify_reason: "",
                refund_error: "",
                track_deviceid: "8EF77D0C-5531-4CD9-8176-6EDC49FFEC03",
                lastalipaydatetime: 1428547778,
                lastminute_title: "409秒杀LM",
                lastminute_price: "1000",
                products_type: 0,
                products_title: "1111",
                alipay_account: "raffi@126.com",
                supplier_title: "自己人",
                supplier_type: 0,
                supplier_phone: "15810922404",
                stock: 197,
                secondpay_start_time: 0,
                secondpay_end_time: 0,
                pay_type: 0,
                room_price_total: 0,
                products_departure_date: "2015/05/09",
                buyerinfo_name: "小美",
                buyerinfo_phone: "18500192000",
                buyerinfo_email: "sunnyding602@qq.com",
                lastminute: {
                    id: "10207",
                    title: "409秒杀LM",
                    product_type: "1785",
                    recommend: "0",
                    views: "19",
                    status: "0",
                    onsale: "1",
                    booktype: "1",
                    supplierid: "1860",
                    sort_time: "0",
                    sort_weight: "0",
                    pay_time: "1428544528",
                    start_time: "1428543682",
                    end_time: "1431619224",
                    travel_starttime: "1428508800",
                    travel_endtime: "1432828800",
                    abroad: "inland",
                    start_pos: "青岛",
                    continent: "a:1:{i:10;a:1:{i:0;s:2:"14";}}",
                    country: "英国",
                    city: "伦敦",
                    poi: "",
                    channel: "web,h5,mobile",
                    modifytime: "1428648572",
                    price: "1000",
                    list_price: "1000",
                    buy_price: "1",
                    feature: "",
                    pic: "http://test1362383214.qiniudn.com/public/lastmin/lastminute/2015/04/10/14286481337359",
                    timeout: "5",
                    soldnum: "0",
                    reservationday: "10",
                    use_if: "",
                    qyer_url: "",
                    url: "",
                    groupno: "",
                    travelday: "0",
                    travelnight: "0",
                    vehiclego: "0",
                    vehicleback: "0",
                    reservationtype: "1",
                    reservationdesc: "",
                    phone: "",
                    plan_id: "0",
                    discount_code: "",
                    order_type: "0",
                    login_visible: "0",
                    supplieradmin: "4632288",
                    adminid: "63",
                    role: "255",
                    end_pos: "英国,伦敦",
                    addtime: "1428543707",
                    modify: "189",
                    supplier: "1860",
                    isnew: "0",
                    start_date: "2015-04-09 09:41:22",
                    end_date: "2015-05-15 00:00:24",
                    pic_info: null,
                    reservationhour: "0",
                    reservationmin: "0",
                    offshelvestype: "1",
                    paymenttype: "1",
                    suppliermodify: "4632288",
                    verifystatus: "2",
                    soldout: "0",
                    csh: "["0571-87356978"]",
                    web_order: "0",
                    wsoldnum: "0",
                    weight: "0",
                    info_give: "",
                    detail_image: null,
                    booking_time: "2015年1月26日至12月31日",
                    travel_time: "",
                    ctn: "12",
                    op_pic: "",
                    op_pic1: "",
                    departure: "青岛",
                    relatid: "",
                    currency_code: "",
                    firstpay_start_time: "1428544528",
                    firstpay_end_time: "0",
                    secondpay_start_time: "0",
                    appoint_date: "0",
                    holiday: "",
                    relatepoi: "",
                    editadmin: "189"
                },
                supplier: {
                    id: "1860",
                    catename: "自己人",
                    catename_en: "test",
                    catename_py: "ceshi",
                    image: "http://test1362383214.qiniudn.com/public/lastmin/supplier/2014/05/30/1401448532",
                    sub_image: null,
                    alipay_account: "raffi@126.com",
                    phone: "15810922404",
                    siteurl: "http://www.qyer.com/",
                    email: "zidong.li@qyer.com",
                    type: "2",
                    status: "1",
                    uid: "5287890",
                    username: "putao888",
                    legal_person: "lilili",
                    full_catename: "呀1212121",
                    gid: "14",
                    show_user_info: "1",
                    submit: "0",
                    submittime: "0",
                    modify: "63",
                    modifytime: "1428384766",
                    royalty_status: "1",
                    complain_phone: "12345678",
                    emergency_phone: "400-1234567"
                },
                products: {
                    id: "1292",
                    lid: "10207",
                    sid: "1860",
                    title: "1111",
                    total: "0",
                    stock: "0",
                    price: "0.00",
                    advance_payment: "0.00",
                    buy_limit: "0"
                },
                orderform: {
                    id: "1996795662",
                    lid: "10207",
                    pid: "1292",
                    cid: "5836",
                    sid: "1860",
                    num: "1",
                    name: "小美",
                    phone: "18500192024",
                    email: "sunny@bunengzhai.com",
                    uid: "5287911",
                    unit_price: "0.01",
                    price: "0.01",
                    payment: "0",
                    datetime: "1428547478",
                    firstpay: "1",
                    relid: null,
                    buyer_email: null,
                    buyer_id: null,
                    notify_id: null,
                    notify_time: null,
                    notify_type: null,
                    payment_type: null,
                    seller_email: null,
                    seller_id: null,
                    sign: null,
                    sign_type: null,
                    total_fee: null,
                    trade_no: null,
                    trade_status: null,
                    return_type: null,
                    return_time: null,
                    channel: "ios",
                    guid: "",
                    confirmstatus: "0",
                    rooms: "0",
                    msg: null,
                    refund_status: null,
                    refund_time: "0",
                    refund_return_time: "0",
                    refund_deal_time: "0",
                    refund_reason: "",
                    refund_verify_reason: "",
                    refund_error: "",
                    track_deviceid: "8EF77D0C-5531-4CD9-8176-6EDC49FFEC03"
                },
                qyer_des: "NTI4NzkxMWMyVnlkbWxqWlQwaWJXOWlhV3hsTG5ObFkzVnlhWFI1Y0dGNUxuQmhlU0ltWDJsdWNIVjBYMk5vWVhKelpYUTlJblYwWmkwNElpWnZkWFJmZEhKaFpHVmZibTg5SWxSWlJWSXhPVGsyTnprMU5qWXlJaVp6ZFdKcVpXTjBQU0kwTURubnA1TG1uWUJNVFNJbWNHRjViV1Z1ZEY5MGVYQmxQU0l4SWlaelpXeHNaWEpmYVdROUluSmhabVpwUURFeU5pNWpiMjBpSm5SdmRHRnNYMlpsWlQwaU1DNHdNU0ltWW05a2VUMGlNVEV4TVNJbWJtOTBhV1o1WDNWeWJEMGlhSFIwY0NVelFTVXlSaVV5Um1Gd2FTNXhlV1Z5TG1OdmJTVXlSbTBsTWtaaGNIQmhiR2x3WVhsdWIzUnBabmt1Y0dod0lpWnBkRjlpWDNCaGVUMGlNakF4TlMwd05DMHdPU0F4TURvME9Ub3pPQ0k9NDRjODZkYmRlNjIzMzQwYjVlMGE="
            }
        ]
    }
}
```


### HTTP Request

`GET http://open.qyer.com/lastminute/app_get_userorderformlist`

### Query Parameters

参数|类型| 必须|默认|描述 
--------- |--------- | --------- | ------- | -----------
**client_id** |String| 是 | 空字符串 | Open平台客户端id
**client_secret**|String| 是| 空字符串 | Open平台客户端密码
**oauth_token**|String| 是| 空字符串 | 采用OAuth授权方式为必填参数， OAuth授权后获得。
is_show_pay|Int| 否| 0| 是否显示支付类(我也没看懂, 目前App传的是1)
`count`|int| 否| 10| 每页显示数量
`page`|int| 否| 1| 页码
`is_show_supplier`|String| 否| 0| 显示供应商创建的折扣 默认值 0:不显示供应商的 1:显示全部
*track_user_id*|String| 否| 空字符串 | 用户UID，未登录传空。（数据中心用）
*track_deviceid*|String| 否| 空字符串 | 设备号。（数据中心用）
*track_app_version*|String| 否| 空字符串 | 当前版本。（数据中心用）
*track_app_channel*|String| 否| 空字符串 | 安装渠道。（数据中心用）
*track_device_info*|String| 否| 空字符串 | 设备型号。（数据中心用）
*track_os*|String| 否| 空字符串 | 操作系统和版本号。（数据中心用）
*app_installtime*|String| 否| 空字符串 | APP安装时间。（数据中心用）


## 折扣筛选/排序接口


```shell
curl "http://open.qyer.com/lastminute/app_get_lastminute_list?oauth_token=e458c75b658c5252c4c115ca737b2053&client_secret=44c86dbde623340b5e0a&client_id=qyer_discount_ios&track_os=ios%25208.3&track_device_info=iPhone%25205(ChinaMobile,ChinaTelecom,ChinaUnicom)&orderValue=0%7C1428465156%7C10161&continent_id=0&track_deviceid=8EF77D0C-5531-4CD9-8176-6EDC49FFEC03&orderName=r0%7Cs1%7Ci2&track_app_version=1.6.3&times=&product_type=0&app_installtime=1421109485&track_app_channel=App%2520Store&track_user_id=5287911&country_id=0"
```

> The above command returns JSON structured like this:

```json
{
    status: 1,
    info: "",
    times: 0,
    data: {
        count: 25,
        orderName: "r0|s1|i2",
        orderValue: "0|1428465156|10161",
        lastminutes: [
            {
                id: "37",
                title: "子冬底层重构自由行00",
                pic: "http://static.qyer.com/upload/lastminute/main/e9/2f/e92fc3818ac72305c6a87921d82d8518_275",
                detail: "",
                price: "<em>5555</em>元起",
                booktype: "1",
                firstpay_end_time: "1450195200",
                end_date: "2015.12.16结束",
                feature: "1022,1023",
                list_price: "99991",
                buy_price: "5555",
                self_use: 1,
                first_pub: 1,
                perperty_today_new: 0,
                lastminute_des: "0.6折",
                url: "http://appview.qyer.com/z/deal/37/"
            },
            {
                id: "10202",
                title: "预定上线审核测试",
                pic: "http://test1362383214.qiniudn.com/public/supplier/lastminute/2015/04/10/14286406837322/600x400",
                detail: "",
                price: "<em>11</em>元起",
                booktype: "1",
                firstpay_end_time: "1431532800",
                end_date: "2015.05.14结束",
                feature: "",
                list_price: "111",
                buy_price: "11",
                self_use: 0,
                first_pub: 0,
                perperty_today_new: 0,
                lastminute_des: "1折",
                url: "http://appview.qyer.com/z/deal/10202/"
            }
        ]
    }
}
```


### HTTP Request

`GET http://open.qyer.com/lastminute/app_lastminute_list`

### Query Parameters
必选    类型及范围  说明

参数|类型| 必须|默认|描述 
--------- |--------- | --------- | ------- | -----------
**client_id** |String| 是 | 空字符串 | Open平台客户端id
**client_secret**|String| 是| 空字符串 | Open平台客户端密码
**oauth_token**|String| 是| 空字符串 | 采用OAuth授权方式为必填参数， OAuth授权后获得。
**`order`**|String| 否| 空字符串|不传采用默认排序, salesAsc(销量正序)  salesDesc(销量倒序) priceAsc(价格正序) priceDesc(价格倒序)  in24(当日新品)
`is_show_pay`|Int| 否| 0|显示支付类 默认值0 不显示支付类 
`product_type`|Int| 否| 0| 分类id 默认值0 指全部分类
`page_size`|int| 否| 10| 每页显示数量
`times`|string| 否| 空字符串| 时间
`continent_id`|int| 否| 10| 大洲id
`country_id`|int| 否| 10| 国家id
`departure`|string| 否| 10|出发城市 
`orderName`|string| 否| 10|排序值对应的排序名称 格式:recommend/id/edittime 
`orderValue`|string| 否| 10|当前列表排序值 格式:推荐值/id值/更新时间戳值 (当页最后一个折扣的推荐值、id值、更新时间值) 
`is_show_supplier`|String| 否| 0| 显示供应商创建的折扣 默认值 0:不显示供应商的 1:显示全部
*track_user_id*|String| 否| 空字符串 | 用户UID，未登录传空。（数据中心用）
*track_deviceid*|String| 否| 空字符串 | 设备号。（数据中心用）
*track_app_version*|String| 否| 空字符串 | 当前版本。（数据中心用）
*track_app_channel*|String| 否| 空字符串 | 安装渠道。（数据中心用）
*track_device_info*|String| 否| 空字符串 | 设备型号。（数据中心用）
*track_os*|String| 否| 空字符串 | 操作系统和版本号。（数据中心用）
*app_installtime*|String| 否| 空字符串 | APP安装时间。（数据中心用）
