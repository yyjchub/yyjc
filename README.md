# V2b-Theme-Sleek

v2b前后端分离主题 Sleek

> 前后端分离主题 可搭建多个前端应用 <br>
> 提交的需求尽量满足 不定期维护更新

## 安装教程
- 后端：修改v2b后端支付回调文件 
  > 前后端分离重要步骤 
  - 进入目录 `app/Services/PaymentService.php`

  - 文件第50行 `'return_url' => config('v2board.app_url') . '/#/order/' . $order['trade_no'],`
  - 修改成：` 'return_url' => $_SERVER['HTTP_ORIGIN'] . "/#/dashboard",` 
  
  <br>
-  前端：正常解析一个网址到解析目录 下载前端文件放置解析根目录
    > 前端配置部分都在config.js 文件里
    - 修改config.js的hosturl 填写后端网址 `https://xxxx.xx/` 格式




