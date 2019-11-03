# Latte：一款清爽、可自定义的SSPANEL主题

## 新版特点

- 去除旧版艳丽色彩，增加无数个可自定义参数的配置文件。
- 新增易支付，可对接任意一家易支付网站或自行搭建一套易支付对接个人的支付宝当面付或个人的小微商户，实现相对安全的收款方式。
- 集成10种支付接口，包含码支付、支付宝当面付、番茄云支付、易支付、 BitPay 、Payjs、Trimepay 、ChenAlipay、Paymentwall、Spay。推荐使用易支付，可一次性解支付宝、微信、QQ三端收款问题。
- 重视细节，无论登录注册、还是404、405、500等异常页面，灵动壁纸，无缝连贯，动态变换。
- 首页模板支持自定义参数、自带两套模板可随意切换。
- 新增自定义全局弹窗公告，适合通知重要内容。
- 新增自定义参数latte_config文件， 可定制外观、开启或关闭相关功能，操作非常方便。
- 注册页移除联系方式等鸡肋功能，网站首页可设置为登录页面。
- 支持多渠道收款，比如当面付和微信payjs和bitpay可共存收款，避免以往仅有一套支付系统可用。
- 支持V2Ray、SS、SSR(即使不开v2ray，其它都可以正常使用)。
- 付费者将享受后续免费升级和维护服务。
- 自带一键部署脚本，只需安装好宝塔+php7.3即可自动完成部署，提供远程指导服务。

## 价格

限时优惠：300元（399元），带域名授权，支持域名变更。已适配一键部署，2分钟可搭建一个新站，5分钟可完成旧站迁移。

购买地址：[佰阅小店](https://mall.baiyue.one)

## 特别优惠

Latte主题 + [rico V2Ray付费版后端](https://github.com/rico93/pay-v2ray-sspanel-v3-mod_Uim-plugin/tree/master)，原价899，现在只需799

Latte主题 + [SSR后端一键对接脚本](https://mall.baiyue.one/product/4.html)，原价550，现在只需450

备注：v2ray对接是绑定域名的；ssr后端对接一键脚本不绑定域名，不限制节点数量。

## 截图

TG联系 [@Latte](https://t.me/Latte_Coffe) 购买或看demo，同时接定制功能

主题基于[Anankke/SSPanel-Uim](https://github.com/Anankke)开发，保持长期维护更新。

[
![Latte：一款优雅和现代时尚的SSPANEL主题](https://baiyue.one/wp-content/uploads/2019/10/2019110316022928.png)](https://baiyue.one/wp-content/uploads/2019/10/2019110316022928.png)

[![Latte：一款优雅和现代时尚的SSPANEL主题](https://baiyue.one/wp-content/uploads/2019/10/20191007084105100.png)](https://baiyue.one/wp-content/uploads/2019/10/20191007084105100.png)

[![Latte：一款优雅和现代时尚的SSPANEL主题](https://baiyue.one/wp-content/uploads/2019/10/2019100708410783.png)](https://baiyue.one/wp-content/uploads/2019/10/2019100708410783.png)

![](https://baiyue.one/wp-content/uploads/2019/10/2019110313544099.png)

![](https://baiyue.one/wp-content/uploads/2019/10/2019110313544391.png)

![](https://baiyue.one/wp-content/uploads/2019/10/2019110313544580.png)

## 自定义参数

.latte_config文件：

```bash
<?php

/*


.__             __     __           
|  |  _____   _/  |_ _/  |_   ____  
|  |  \__  \  \   __\\   __\_/ __ \ 
|  |__ / __ \_ |  |   |  |  \  ___/ 
|____/(____  / |__|   |__|   \___  >
           \/                    \/ 

                  made by @latte_coffe

*/

// 通用设置：'true'代表开启；'false' 代表关闭。
// 版本信息说明（请勿更改）
$Latte_Config['version'] = '1.0.3';
$Latte_Config['index_style'] = 'index';  //网站首页模板选择，index：默认模板；login：登陆页模板。

// 网站首页
$Latte_Config['index_logo'] = 'Latte_Coffe';  //网站首页logo,尽量简短的两三个字母，效果最佳
$Latte_Config['index_slogan'] = '全球中继服务，更快更稳'; //网站首页标语（不超过10个效果最佳）


//网站首页细节设置(必须为纯数字)
$Latte_Config['index_location'] = '200'; //服务地区数量
$Latte_Config['index_node'] = '20'; //节点数量
$Latte_Config['index_device'] = '10'; //终端数量
$Latte_Config['index_user'] = '130'; //用户数量

//网站首页价格
$Latte_Config['stand_price_mo'] = '10'; //服务地区数量
$Latte_Config['stand_price_sea'] = '25'; //节点数量
$Latte_Config['stand_price_year'] = '100'; //终端数量
$Latte_Config['pro_price_mo'] = '25'; //服务地区数量
$Latte_Config['pro_price_sea'] = '70'; //节点数量
$Latte_Config['pro_price_year'] = '260'; //终端数量

// 用户首页
$Latte_Config['enable_public_tos'] = false; //用户页自定义弹窗公告，用于紧急通知或者其它用途
$Latte_Config['public_notice'] = '这里是弹窗公告';  //弹窗通知：仅在有重大通知时使用，否则会降低用户体验

// 订阅设置
$Latte_Config['enable_sub_ss'] = false;    // 是否启用ss/ssd订阅按钮
$Latte_Config['enable_sub_ssr'] = true;   // 是否启用ssr订阅按钮，此按钮为合并后的订阅链接，包含普通端口和单端口，如果需要分开显示单端口和普通端口，请关闭此选项，开启以下按钮
$Latte_Config['enable_sub_ssr_single'] = false; // 是否启用ssr单端口订阅按钮，如果开启，请关闭上面的按钮
$Latte_Config['enable_sub_ssr_normal'] = false; // 是否启用ssr普通口订阅按钮
$Latte_Config['enable_sub_v2ray'] = true; // 是否启用v2订阅按钮
$Latte_Config['enable_sub_clash'] = true; // 是否启用clash订阅按钮

// 客户端设置
$Latte_Config['enable_ssr'] = true;  //是否启用ssr客户端,作用于用户页面板右下角的客户端下载
$Latte_Config['enable_v2ray'] = true; //是否启用v2ray客户端


// 左侧菜单设置
$Latte_Config['enable_list'] = true;  //是否启用趣味排行榜，主要为前十流量统计、邀请统计，自动去除敏感信息
$Latte_Config['enable_lookingglass'] = true; //是否启用延迟检测，数据来源speedtest
$Latte_Config['enable_ticket'] = true; //是否启用工单系统
$Latte_Config['enable_trafficlog'] = false; //是否启用72h个人流量使用记录

// 其它设置：登陆/注册背景修改位置/public/theme/latte/images/user_bg.jpg；用户界面顶部背景图修改，同上。
```

