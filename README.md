# EasyPhotos    
[![](https://jitpack.io/v/HuanTanSheng/EasyPhotos.svg)](https://jitpack.io/#HuanTanSheng/EasyPhotos)    

QQ交流群：[288600953](https://jq.qq.com/?_wv=1027&k=5QGgCDe)    

  


| 无选中状态（默认UI色调）   | 选中状态（ [自定义UI色调](https://github.com/HuanTanSheng/EasyPhotos/wiki/10-%E8%87%AA%E5%AE%9A%E4%B9%89UI%E6%A0%B7%E5%BC%8F)）  | 其他功能（各功能可自选） |
|:-----------:|:--------:|:---------:|
|![](images/01.png) | ![](images/02.png) | ![](images/03.png)|  

| 专辑列表（默认UI色调） | 相册带广告（ [自定义UI色调](https://github.com/HuanTanSheng/EasyPhotos/wiki/10-%E8%87%AA%E5%AE%9A%E4%B9%89UI%E6%A0%B7%E5%BC%8F)） | 专辑列表带广告 |
|:-------:|:---------:|:---------:|
|![](images/05.png) | ![](images/04.png) | ![](images/06.png)|  

| 预览页   |  预览页单击图片转全屏模式 | 预览页缩放图片 | 
|:-------:|:---------:|:---------:|
|![](images/07.png) | ![](images/08.png) | ![](images/09.png)|   

|预览页单击缩放图片显示操作栏 | 拼图选择页| 拼图选择页 |
|:-------:|:---------:|:---------:|
|![](images/10.png) | ![](images/11.png) | ![](images/12.png)|     

|拼图页 | 拼图页拼图功能| 拼图页文字贴纸功能 |
|:-------:|:---------:|:---------:|
|![](images/13.png) | ![](images/14.png) | ![](images/15.png)|     

|文字贴纸编辑页 | 示例功能列表 | 示例功能列表 |
|:-------:|:---------:|:---------:|
|![](images/16.png) | ![](images/17.png) | ![](images/18.png)|    
    
    
## 产品特色    
- 支持绑定Glide、Picasso、Fresco、Imageloader等所有图片加载库，EasyPhotos并没有对他们进行依赖，不必担心冲突和体积问题。     
- 状态栏字体颜色智能适配，当状态栏颜色趋近于白色时，字体颜色智能处理为深色     
- 内部处理运行时权限，使用者无需考虑权限问题    
- 拼一张功能（可配置开关，可独立作为拼图使用）    
- 原图功能（可配置开关）    
- 广告填充（可配置开关）     
- 过滤图片（图片宽度、图片高度、文件大小三个维度任意选择和搭配）
- 默认勾选图片（可配置）    
- 图片预览（可全屏，可缩放）    
- UI色值高度浓缩，仅为7种，自定义超简单     
- 对Gif动图的处理（可配置开关是否显示，列表中以静态图+动图标识显示，预览大图时自动播放）    
- 自带Bitmap相关方法（如添加水印、把View画成Bitmap、保存Bitmap等）    
- 自带媒体库相关方法（如媒体文件更新到媒体库）    

## 关于EasyPhotos的SDK及相关版本公示 
compileSdkVersion 27  
minSdkVersion 15  
targetSdkVersion 27      
buildToolsVersion '27.0.3'    
QQ交流群：[288600953](https://jq.qq.com/?_wv=1027&k=5QGgCDe)    


## 获取EasyPhotos（通过Gradle方式）
首先，在项目的 `build.gradle（project）` 文件里面添加:

```gradle
allprojects {
	repositories {  

        maven { url "https://jitpack.io" }
		
    }
}
```

最后，在你需要用到EasyPhotos的module中的 `build.gradle（module）` 文件里面添加：
```gradle
dependencies {  

    implementation 'com.github.HuanTanSheng:EasyPhotos:2.2.8'  
    
}
```    
    
    


    
       
**如果你的 `android studio` 版本不同于3.0.1正式版，有可能会打不开我的Demo，只需要修改Demo里面 `build.gradle（project）` 文件中的：**     

```gradle  

dependencies {
        classpath 'com.android.tools.build:gradle:3.0.1'
	//把3.0.1改成你对应的版本即可，如果不清楚对应版本可以看看你其他正常项目的这里是怎么写的  
	}

```    
    
## 关于混淆    
  
**EasyPhotos的混淆：**  
```pro  

-keep class com.huantansheng.easyphotos.models.** { *; }

```

    
    
  
## EasyPhotos文档总录    

## [EasyPhotos文档总录](https://github.com/HuanTanSheng/EasyPhotos/wiki)
* [01-关于权限](https://github.com/HuanTanSheng/EasyPhotos/wiki/01-%E5%85%B3%E4%BA%8E%E6%9D%83%E9%99%90)
* [02-相机与相册](https://github.com/HuanTanSheng/EasyPhotos/wiki/02-%E7%9B%B8%E6%9C%BA%E4%B8%8E%E7%9B%B8%E5%86%8C)    
* [03-拼图（单独使用）](https://github.com/HuanTanSheng/EasyPhotos/wiki/03-%E6%8B%BC%E5%9B%BE%EF%BC%88%E5%8D%95%E7%8B%AC%E4%BD%BF%E7%94%A8%EF%BC%89)      
* [04-图片添加水印](https://github.com/HuanTanSheng/EasyPhotos/wiki/04-%E5%9B%BE%E7%89%87%E6%B7%BB%E5%8A%A0%E6%B0%B4%E5%8D%B0)     
* [05-把View画成Bitmap](https://github.com/HuanTanSheng/EasyPhotos/wiki/05-%E6%8A%8AView%E7%94%BB%E6%88%90Bitmap)    
* [06-保存Bitmap到指定文件夹](https://github.com/HuanTanSheng/EasyPhotos/wiki/06-%E4%BF%9D%E5%AD%98Bitmap%E5%88%B0%E6%8C%87%E5%AE%9A%E6%96%87%E4%BB%B6%E5%A4%B9)    
* [07-Bitmap回收](https://github.com/HuanTanSheng/EasyPhotos/wiki/07-Bitmap%E5%9B%9E%E6%94%B6)
* [08-更新媒体文件到媒体库](https://github.com/HuanTanSheng/EasyPhotos/wiki/08-%E6%9B%B4%E6%96%B0%E5%AA%92%E4%BD%93%E6%96%87%E4%BB%B6%E5%88%B0%E5%AA%92%E4%BD%93%E5%BA%93)
* [09-屏幕方向设置](https://github.com/HuanTanSheng/EasyPhotos/wiki/09-%E5%B1%8F%E5%B9%95%E6%96%B9%E5%90%91%E8%AE%BE%E7%BD%AE)
* [10-自定义UI样式](https://github.com/HuanTanSheng/EasyPhotos/wiki/10-%E8%87%AA%E5%AE%9A%E4%B9%89UI%E6%A0%B7%E5%BC%8F)
* [11-多语言](https://github.com/HuanTanSheng/EasyPhotos/wiki/11-%E5%A4%9A%E8%AF%AD%E8%A8%80)      
* [12-配置ImageEngine，支持所有图片加载库](https://github.com/HuanTanSheng/EasyPhotos/wiki/12-%E9%85%8D%E7%BD%AEImageEngine%EF%BC%8C%E6%94%AF%E6%8C%81%E6%89%80%E6%9C%89%E5%9B%BE%E7%89%87%E5%8A%A0%E8%BD%BD%E5%BA%93)

    
QQ交流群：[288600953](https://jq.qq.com/?_wv=1027&k=5QGgCDe)    
    
       
           
	   
## 感谢    


[Glide](https://github.com/bumptech/glide)：我心目中最好的图像加载和缓存库，由[Bump Technologies](https://github.com/bumptech) 团队编写。已经从EasyPhotos中去除依赖，大家可以通过ImageEngine接口实现任意图片加载库的绑定。    

[PhotoView](https://github.com/chrisbanes/PhotoView)：一个强大的图片缩放库，由[chrisbanes](https://github.com/chrisbanes) 大神编写    
    
[PuzzleView](https://github.com/wuapnjie/PuzzleView)：一个强大的拼图库，我的拼图功能是在此基础上实现，这个库由[wuapnjie](https://github.com/wuapnjie) 编写。    
    
## 编者语    

EasyPhotos将在高颜值、高兼容、高性能、强功能的道路上持续更新，欢迎各种Issues，我将及时反馈，谢谢！    
QQ交流群：[288600953](https://jq.qq.com/?_wv=1027&k=5QGgCDe)      


## 更新日志      

**2.2.8：**    
- bug修复：在预览页点击最后一张的选择无效，以及因此产生的数组越界bug    
- bug修复：极少情况下的预览页直接返回产生的空指针问题    
- 感谢@zijinzhiyun 反馈以上bug
    
    
**2.2.6：**    
- api修改：为统一api标准，将所有返回Key统一为EasyPhotos.RESULT_PHOTOS和EasyPhotos.RESULT_PATHS。带来的改变就是单独使用拼图功能时的图片返回Key改为EasyPhotos.RESULT_PHOTOS和EasyPhotos.RESULT_PATHS，去除原来的EasyPhotos.RESULT_PUZZLE_PHOTO和-
EasyPhotos.RESULT_PUZZLE_PATH这两个Key。      
- UI修改：预览页状态栏颜色与colorPrimaryDark色值对应。若其色值趋近于白色，在无虚拟按键的手机中状态栏字体颜色智能适配为深色，有虚拟按键的手机中状态栏智能优化为透明色。（除预览页外，其他页面若状态栏颜色趋近于白色，无论任何机型均为智能优化字体颜色为深色，[查看详情。](https://github.com/HuanTanSheng/EasyPhotos/wiki/10-%E8%87%AA%E5%AE%9A%E4%B9%89UI%E6%A0%B7%E5%BC%8F)）     
- 错误修复：修复努比亚机型的预览页占用导航栏问题      

**2.2.4：**    
- 优化：单独启动相机时无需配置图片加载引擎       
- 优化：示例中配置Glide4.x为图片加载引擎的示例文件改为单例模式    

**2.2.3：**    
- 修复拼一张更换图片时发生的错误    
- 修复单独启动相机时的权限错误    
- 优化混淆规则    

**2.2.2：**    
- 重大更新：EasyPhotos去除了Glide的依赖，并对外提供ImageEngine接口，通过对ImageEngine接口的实现，使用者可以快速绑定如Glide、picasso、fresco、Imageloader等你正在使用的任意图片加载库。[点击查看详情](https://github.com/HuanTanSheng/EasyPhotos/wiki/12-%E9%85%8D%E7%BD%AEImageEngine%EF%BC%8C%E6%94%AF%E6%8C%81%E6%89%80%E6%9C%89%E5%9B%BE%E7%89%87%E5%8A%A0%E8%BD%BD%E5%BA%93)    
- 界面优化：优化单选图标    
- 修改文字贴纸的文字编辑页面中，底部操作栏的背景色为固定色值（其实也可以改，看看EasyPhotos的color文件你就知道怎么改）

    
**2.1.0：**    
- 新增功能：EasyPhotos智能识别状态栏的背景颜色，当其趋近于白色时，智能适配深色状态栏字体。（该功能仅对6.0以上系统生效，并没有适配6.0以下的小米和魅族，如有需要可以加群交流）    
- 新增功能：可配置是否显示Gif动图    
- 功能优化：Gif动图的处理方式。
- 界面优化：Gif动图、相机按钮等。
- 新增字段：    
````java    
<string name="gif_easy_photos">动图</string>    
````    
具体查看[11-多语言](https://github.com/HuanTanSheng/EasyPhotos/wiki/11-%E5%A4%9A%E8%AF%AD%E8%A8%80)    

- 内部升级：最新版编译工具和最新版sdk

**2.0.2：**    
- 升级：Glide到4.5.0（不影响低版本使用）    
- 修复：拼一张功能因图片过多过大导致的oom问题    
- 感谢@[Beiler](https://github.com/beiler) 提出的反馈      
    
    
**2.0.1：**    
- 修复bug：单独使用拼图功能时，以图片路径为参数时产生的数组越界bug。   

**2.0.0：**   
- 新增功能：相册内部自带拼一张功能（可通过配置不使用该功能，该模式拼图保存的图片存储在 sd卡根目录/你的app_name 文件夹下）   
- 新增功能：拼图页面增加文字贴纸功能    
- 界面优化：无权限时的相册界面优化，使之更加友好    
- 界面优化：相机按钮优化，视觉和体验上都更加友好    
- 界面优化：专辑列表细节优化，更加自然、大气     
- 功能优化：相册界面打开相机，拍照后不直接返回，而是默认选中拍完的图片，停留在相册界面
- 字段增加：具体查看[11-多语言](https://github.com/HuanTanSheng/EasyPhotos/wiki/11-%E5%A4%9A%E8%AF%AD%E8%A8%80)      
- 重要修改：Photo对象去除isCamera成员变量。构造函数也因此相应改变，少了一个参数。
- 重要修改：setFileProviderAuthoritiesText（）方法更改为setFileProviderAuthority（）方法    
- 重要修改：UI色值重新定义，由原来的三十几种色值统一修改为7个色值，自定义起来更加方便。具体查看[10-自定义UI样式](https://github.com/HuanTanSheng/EasyPhotos/wiki/10-%E8%87%AA%E5%AE%9A%E4%B9%89UI%E6%A0%B7%E5%BC%8F)



**1.3.2：**   
- 新增功能：    
    - 拼图（最多对9张图片进行拼图，无需关心运行时权限，内部处理好了）    
    - 把View画成Bitmap    
    - 保存bitmap到本地（可设置是否更新到媒体库，如果调用此方法前没有进入过EasyPhotos的相册或相机，则需要你自己处理读写权限）      
- 更换相册单选的选中图标样式    
- 修复回调选中地址的key：RRESULT_PATHS 修复为 RESULT_PATHS。（ps：对如此智障的疏忽表示歉意。）    
- 修复永久不给权限情况下，退出相册时发生的错误    
- 修复调用系统权限设置页返回时，相册页面或拼图页面自销毁情况
- 新增字符串：    
```java    
    <string name="done_easy_photos">完成</string>
    <string name="cancel_easy_photos">取消</string>
    <string name="template_easy_photos">模板</string>    
```   
- 新增色值：    
```java   
    <!--图片预览页-->
    <color name="preview_status_easy_photos">#d73c3d41</color>//api21以上预览页状态栏颜色为该色值；api19和api20状态栏为透明色；其余api状态栏或透明或黑或灰，取决于各家rom和有无实体按键等因素。注：其余页面状态栏根据你的主题走

    <!--拼图页-->
    <color name="puzzle_background_easy_photos">#000000</color>//拼图页面背景色
    <color name="puzzle_selected_frame_easy_photos">#57a457</color>//拼图页面当前处理item的边框颜色
    <color name="puzzle_selected_controller_easy_photos">#00AA00</color>//拼图页面当前处理item的操作bar颜色，就是item边框中凸起矩形的色值
    <color name="puzzle_menu_easy_photos">#969696</color>//拼图页面的文字按钮和示例图片颜色
    <color name="puzzle_menu_done_easy_photos">#009700</color>//拼图页面的完成按钮文字颜色
    <color name="puzzle_bottom_bar_line_easy_photos">#ee3a3a3e</color>//拼图的底部栏间隔颜色
    <color name="puzzle_photo_background">#ffffff</color>//图片的背景颜色    
```
    
**1.2.8：**    
- 修复'选中图片列表'点击状态下与'大图列表和选择器'的联动错误    

**1.2.7：**    
- 大图预览页新增：大图列表与选中图片列表联动    
- 升级 classpath 'com.android.tools.build:gradle:3.0.1'    
- 新增色值：    
```java    
<color name="preview_bottom_bar_easy_photos">#eb212123</color>//预览页的底部栏和选中图片列表背景颜色    
<color name="preview_bottom_bar_line_easy_photos">#ee3a3a3e</color>//预览页的底部栏与选中图片列表的分割线颜色    
```   

**1.2.6：**    
- 正式开放，投入使用   
- 广告view可以传空，适用于VIP不显示广告场景

**1.2.3：**    
- 优化图片限制方式：最小宽度、最小高度、最小文件大小    
- 如果单一设置，满足条件即过滤    
- 如果多项设置，满足一项即过滤    

**1.2.2：**     
- 新增返回结果：图片地址集合   
- 新增返回结果：用户是否选中原图选项    
- 新增返回结果：图片信息集合    
- 新增设置默认勾选图片集合方式：图片地址集合   
- 新增设置默认勾选图片集合方式：图片信息集合   

**1.2.1：**   
- 优化预览界面全屏动效
- 优化Photo实体对象  

**1.2.0：**   
- 升级图片选取返回信息（图片地址/宽高/文件大小/文件修改时间/文件类型/用户是否点击原图选项/文件名）
- 图片选择新增原图选项
- 预览界面支持选择完成
- 预览界面支持当前图片位置显示   

**1.1.1：**   
- 优化相机和相册的调用API，使之更加友好    

**1.1.0：**   
- 增加图片添加水印功能  
- 增加媒体文件更新到媒体库功能

**1.0.9：**   
- 优化三星部分机型因图片更新到媒体库时没有更新宽高信息时EasyPhotos相册不显示该图片问题

**1.0.8：**   
- 优化自定义UI和多语言

**1.0.7：**   
- 性能优化

**1.0.6：**   
- 修复华为VNS-L31机型拍照无返回问题

**1.0.5：**   
- 修复拍照切换横竖屏发生内存泄漏
- 修复切换语言时产生错误
- 升级glide为最新版4.3.0   

**1.0.4：**    
- 直接启动相机  
- 相册单选  
- 相册多选  
- 相册中支持添加自定义广告  
- 图片预览（缩放/全屏）
- UI可定制  
- 根据图片宽高进行过滤 
- 修复无图片显示时的异常    
- 内部处理权限问题，无需配置，无需处理运行时权限
    
    
    

  

