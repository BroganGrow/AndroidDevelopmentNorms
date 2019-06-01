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
    - [sytles](#sytles)
  - [xml](#xml)
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

|控件状态限定词|说明|
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

整体效果

|模块|业务功能描述|控件描述|控件状态限定词 |例子|
|----|----|-----|----|----|
|登录|QQ登录|ImageView|normal|login_qq_iv_normal.png|
|登录|微信登录|ImageView|normal|login_weixin_iv_normal.png|
### 4.2 Drawable Resource File (.xml)

|    |模块|业务功能描述|控件描述|元素|例子|
|----|----|----|-----|----|-----|
|**形状**|登录|登录按钮|Button|shape|login_enter_btn_shape|
|**选择器**|主模块|底部栏中的首页图标|TextView|selector|main_home_tv_selector|
|**图层**|----|----|-----|layer-list|-----|



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
|**ListView**    |店铺|店铺列表||store_recycle_item_storeinfo|
|                |店铺|店铺列表|头部|store_recycle_header_storeinfo|
|                |店铺|店铺列表|尾部|store_recycle_footer_storeinfo|
|**GridView**|||||


## menu

## mipmap

## navigation

## raw

## transition

## value
### colors
### dimens
### Strings
### sytles

## xml