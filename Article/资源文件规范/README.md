# Resource 资源文件规范
- [Resource 资源文件规范](#resource-资源文件规范)
  - [1.anim](#1anim)
  - [2.animtor](#2animtor)
  - [3.color](#3color)
  - [4.drawable](#4drawable)
    - [4.1 图片文件(.png/.jpg)](#41-图片文件pngjpg)
    - [4.2 Drawable Resource File (.xml)](#42-drawable-resource-file-xml)
  - [font](#font)
  - [interpolator](#interpolator)
  - [layout](#layout)
  - [menu](#menu)
  - [mipmap](#mipmap)
  - [navigation](#navigation)
  - [raw](#raw)
  - [transition](#transition)
  - [value](#value)
    - [colors](#colors)
    - [dimens](#dimens)
    - [Strings](#strings)
    - [styles](#styles)
  - [xml](#xml)
  - [id命名](#id命名)
    - [--->回到目录](#---回到目录)
## 1.anim
## 2.animtor
## 3.color
> 命名规则：模块名_逻辑名称_颜色
## 4.drawable
### 4.1 图片文件(.png/.jpg)
> 命名规则：模块名_业务功能描述_控件描述_控件状态限定词   
- 模块名：项目模块，如登录模块（login）、个人中心（mine）等   
- 业务功能描述：如登录中的QQ登录（qq）  
- 控件描述：参考控件表  
- 控件状态限定词：如，normal（标准）、pressed（按压）、selected（选中）、

|状态限定词|说明|
|----|-----|
|normal（不需要设置state_xxx）|默认状态效果|
|state_selected|选中效果|
|state_accelerated|-----|
|state_activated|激活效果|
|state_active||
|state_checkable|可选效果|
|state_checked|选中效果|
|state_drag_can_accept|-----|
|state_drag_hovered|-----|
|state_enabled|是否可用效果|
|state_first|-----|
|state_focused|聚焦效果|
|state_hovered|悬停效果|
|state_last|-----|
|state_middle|-----|
|state_pressed|-----|
|state_single|-----|
|state_window_focused|窗口聚焦效果|


- 普通

|模块名|控件|逻辑名|例子|
|----|----|-----|----|
|首页|ImageView|定位|home_iv_location.png|
|门店|Button|分享|store_btn_share.png|

- 多状态

|模块名|控件|逻辑名|状态限定词 |例子|
|----|----|-----|----|----|
|主模块|ImageView|首页|normal|main_iv_home_normal.png|
|主模块|ImageView|首页|pressed|main_iv_home_pressed.png|


### 4.2 Drawable Resource File (.xml)

|模块名|元素|控件|逻辑名|例子|
|----|----|-----|----|-----|
|登录|shape|Button|登录按钮|login_shape_btn_login|
|搜索|shape|EditText|搜索栏|search_shape_et_bg|
|我的|shape|View|布局灰色分割线|mine_shape_view_divider_gray|
|-|||||
|主模块|selector|首页图标|TextView|main_selector_tv_home|
|地址|selector|地址标签|Button|main_selector_btn_home|
|-|||||
| |layer-list||| |

对于其他模块都经常需要用到的文件，可以进行提取




## font

## interpolator

## layout

|    |模块|业务功能描述|其他元素|例子|
|----|----|----|-----|----|
|**Activity**|主入口|主页面||main_acitivity_main|
|            |登录|注册页面||login_activity_register|
|**Fragment**|主入口|首页||main_fragment_home|
|**Dialog**|||||
|**include**|||||
|**RecyclerView**|店铺|店铺列表||store_recycle_item_storeinfo|
|                |店铺|店铺列表|头部|store_recycle_header_storeinfo|
|                |店铺|店铺列表|尾部|store_recycle_footer_storeinfo|
|**ListView**    |商品|商品列表||goods_lit_item_storeinfo|
|                |商品|商品列表|头部|goods_list_header_storeinfo|
|                |商品|商品列表|尾部|goods_list_footer_storeinfo|
|**GridView**|||||
|**自定义View**||标题栏||custom_title_bar|


## menu

## mipmap

## navigation

## raw

## transition

## value
### colors

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="colorPrimary">#008577</color>
    <color name="colorPrimaryDark">#00574B</color>
    <color name="colorAccent">#D81B60</color>

    <!--basic colors 基础颜色-->
    <color name="red">#FF0000</color><!--红色-->
    <color name="orange">#FFA500</color><!--橙色-->
    <color name="yellow">#FFFF00</color><!--黄色-->
    <color name="green">#008000</color><!--绿色-->
    <color name="cyan">#00FFFF</color><!--青色-->
    <color name="blue">#0000FF</color><!--蓝色-->
    <color name="purple">#800080</color><!--紫色-->

    <color name="white">#FFFFFFFF</color><!--白色-->
    <color name="black">#000000</color><!--黑色-->
    <color name="gray">#808080</color><!--灰色-->
    <color name="silver">#C0C0C0</color><!--银色-->
    <color name="pink">#FFC0CB</color><!--粉红色-->
    <color name="gold">#FFD700</color><!--金色-->
    <color name="transparent">#00000000</color><!--透明色-->


    <!-- default colors 默认颜色（设计图常用的默认颜色、如字体、提示）-->
    <color name="default_tv_black">#2B2B2B</color>
    <color name="default_tv_gray">#6A6A6a</color>
    <color name="default_bg_gray">#f2f2f2</color>



    <!--默认灰色字体-->
</resources>

```
### dimens

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>


    <!--font size-->
    <dimen name="font_10">10sp</dimen>
    <dimen name="font_11">11sp</dimen>
    <dimen name="font_12">12sp</dimen>
    <dimen name="font_13">13sp</dimen>
    <dimen name="font_14">14sp</dimen>
    <dimen name="font_15">15sp</dimen>
    <dimen name="font_16">16sp</dimen>
    <dimen name="font_17">17sp</dimen>
    <dimen name="font_18">18sp</dimen>
    <dimen name="font_19">19sp</dimen>
    <dimen name="font_20">20sp</dimen>
    <dimen name="font_21">21sp</dimen>
    <dimen name="font_22">22sp</dimen>
    <dimen name="font_23">23sp</dimen>
    <dimen name="font_24">24sp</dimen>


    <!--view spacing-->
    <dimen name="spacing_half">0.5dp</dimen>
    <dimen name="spacing_0">0dp</dimen>
    <dimen name="spacing_1">1dp</dimen>
    <dimen name="spacing_2">2dp</dimen>
    <dimen name="spacing_3">3dp</dimen>
    <dimen name="spacing_4">4dp</dimen>
    <dimen name="spacing_5">5dp</dimen>
    <dimen name="spacing_6">6dp</dimen>
    <dimen name="spacing_8">8dp</dimen>
    <dimen name="spacing_10">10dp</dimen>
    <dimen name="spacing_12">12dp</dimen>
    <dimen name="spacing_15">15dp</dimen>
    <dimen name="spacing_20">20dp</dimen>
    <dimen name="spacing_30">30dp</dimen>


    <!--view width-->
    <dimen name="measure_width_0">0dp</dimen>
    <dimen name="measure_width_100">100dp</dimen>
    <dimen name="measure_width_200">200dp</dimen>
    <dimen name="measure_width_250">250dp</dimen>
    <dimen name="measure_width_300">300dp</dimen>
    <dimen name="measure_width_350">350dp</dimen>

    <!--view height-->
    <dimen name="measure_height_0">0dp</dimen>
    <dimen name="measure_height_48">48dp</dimen>
    <dimen name="measure_height_50">50dp</dimen>
    <dimen name="measure_height_100">100dp</dimen>


</resources>
```
### Strings
> 命名规则：模块名_逻辑名


注：逻辑名单词多的可以用下划线分开,默认数值

|模块名|逻辑名|例子|
|----|---|----|
|主模块|首页|main_home|
|主模块|个人中心|main_mine|
|-|||
|我的|收益明细|mine_income|
|我的|查看全部订单|mine_check_all_order|
|-|||
|钱包|余额|wallet_default_balance|
|钱包|用户名|wallet_default_username|


### styles
如何从现有的布局中快速高效地提取Style

对于同一个view相似的写法可以提出为style
## xml

## id命名
> 命名规则：控件缩写_模块名_逻辑名

此外，对于布局中不需要用到的，尽量不用添加id；对于第三方的控件同样采用驼峰缩写；同时利用`模块名`搜索时可以轻松过滤掉重复的id；

|控件|模块名|逻辑名|例子|
|------|---|-----|-----|
|Button|个人中心|settings|btn_mine_settings|
|TextView|首页|name|tv_home_name|




### [--->回到目录](/README.md)