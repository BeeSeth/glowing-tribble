# HBuilder X - Release Notes
======================================
## 3.7.0.20230118-alpha
### HBuilder
* 修复 某些情况下，因编辑器主题配置异常，导致HBuilderX无法启动的Bug
* 修复 语言服务 Vue文件，当只有script和style节点，没有template节点时，文档结构图显示空白的Bug
* 修复 Markdown code区域无法高亮显示空白字符的Bug
* 修复 Markdown 从WPS复制表格数据粘贴为Markdown表格语法转换错误的Bug
* 修复 查找索引符号 按下esc取消后，编辑器不会自动滚动到原来的光标所在位置的Bug
* 修复 uniCloud 云函数 当云函数目录下存在中文文件时，上传并运行操作失败的Bug
* 新增 App真机运行 MacOSX 运行项目到iOS真机，自动启动App （需MacOSX安装跟iOS手机系统相匹配的Xcode）[详情](https://uniapp.dcloud.net.cn/tutorial/run/run-app.html#ios-app-automatically-open)
* 新增 App真机运行 Windows iOS标准基座 支持使用Apple证书签名，签名后可运行标准基座到iOS真机设备 [详情](https://uniapp.dcloud.net.cn/tutorial/run/ios-apple-certificate-signature.html)
* 新增 App真机运行 Windows 设备选择窗口 基座选择列表，自定义基座和标准基座支持使用&快捷键进行切换
* 新增 uni-app 微信小程序发行，自动上传到微信平台，支持配置微信ci机器人编号 [详情](https://uniapp.dcloud.net.cn/tutorial/build/publish-mp-weixin-cli.html)
* 新增 uni-app uts插件 运行到Android支持debug调试 [详情](https://uniapp.dcloud.net.cn/tutorial/debug/uni-uts-debug.html)
* 优化 uni-app uts插件 iOS编译，提升编译速度
### uni-app插件
* 【重要】新增 uts 组件。可使用uts语言开发原生扩展组件 [详情](https://uniapp.dcloud.net.cn/plugin/uts-component.html)
* 新增 uni-vue-devtools 插件，方便查看、修改 data 及审查自定义组件 [详情](https://uniapp.dcloud.net.cn/tutorial/debug/uni-vue-devtools.html)
* Web平台、App平台 新增 page-meta 组件支持 scroll-top 属性
* Web平台 修复 3.6.16版引出的 Vue3 项目 scroll-view 组件插槽部分情况下渲染异常的Bug [详情](https://ask.dcloud.net.cn/question/149557)
* Web平台 修复 video 组件 show-progress 属性不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3908)
* Web平台 修复 input 组件 type=digit 时清空输入框后 placeholder 不显示的Bug [详情](https://ask.dcloud.net.cn/question/160726)
* Web平台 修复 Vue3 项目 onNavigationBarSearchInputConfirmed 无效的Bug [详情](https://ask.dcloud.net.cn/question/154740)
* Web平台 修复 Vue3 项目切换 tabbar 页面不触发 onTabItemTap 的Bug
* App平台 新增 【ext component】animation-view 组件 [详情](https://uniapp.dcloud.net.cn/component/animation-view.html)
* App平台 修复 Vue3 项目中原生导航栏 type 为 transparent 时，自定义 buttons 在导航栏上滑至顶端时颜色不改变的Bug [详情](https://ask.dcloud.net.cn/question/154074)
* 小程序平台 新增 pages.json 支持配置 entryPagePath 属性 [详情](https://ask.dcloud.net.cn/question/126216)
* 微信小程序平台 修复 3.6.16版引出的企业版微信运行报错的Bug
* 微信小程序平台 修复 3.6.16版引出的 Vue2 项目部分情况下作用域插槽中访问 length 属性报错的Bug
* 微信小程序平台 修复 Vue2 项目中使用 uni.env 时返回值不正确的Bug [详情](https://ask.dcloud.net.cn/question/159865)
* 支付宝小程序平台 修复 钉钉小程序使用 uni.saveImageToPhotosAlbum 报错的Bug [详情](https://ask.dcloud.net.cn/question/159183)
* 支付宝小程序平台 修复 uni.getSystemInfo 返回的 platform 属性在模拟器中不正确的Bug
* QQ小程序平台 修复 Vue3 项目 video 组件 ended 事件在真机不触发的Bug [详情](https://ask.dcloud.net.cn/question/155602)
### uniCloud插件
* 新增 schema扩展js支持引入公共模块及扩展库 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql.html#deps-of-jql)
* 新增 JQL触发器方法新增一些参数 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#trigger-param)
### App插件(含5+App和uni-app的App端)
* Android平台 新增 隐私政策提示框支持 backToExit 配置是否响应点击系统返回键退出应用，解决部分应用市场上架审核可能提示`系统返回键失灵`的问题 [详情](https://uniapp.dcloud.net.cn/tutorial/app-privacy-android.html)
* Android平台 更新 uni-AD 腾讯优量汇广告SDK 为 4.500.1370 版；Sigmob广告联盟SDK 为 4.9.0 版
* Android平台 修复 3.6.17版引出的 系统导航栏按键颜色与背景颜色相同的Bug [详情](https://ask.dcloud.net.cn/question/161501)
* Android平台 修复 3.6.17版引出的 自定义隐私政策提示框时启动应用可能出现卡死的Bug [详情](https://ask.dcloud.net.cn/question/161634)
* Android平台 修复 隐私合规检测可能报`隐私弹窗中处理超链接的过程中调用到了获取设备sim卡国家信息的api`的Bug [详情](https://ask.dcloud.net.cn/question/161479)
* Android平台 修复 图片选择在 Android13 设备提示没有权限的Bug [详情](https://ask.dcloud.net.cn/question/160879)
* Android平台 修复 plus.io.FileReader 的 readAsDataURL 读取数据时未按 slice 分割位置读取的Bug [详情](https://ask.dcloud.net.cn/question/160467)
* Android平台 修复 视频播放控件 VideoPlayer 在视频缓冲时触发 timeupdate 事件的Bug
* iOS平台 更新 一键登录使用的个验SDK为 3.0.3.0 版
### uni小程序SDK
* Android平台 修复 打开uni小程序切换应用到后台运行一段时间后可能引起崩溃的Bug [详情](https://ask.dcloud.net.cn/question/141868)

## 3.6.17.20230111-alpha
### uni-app插件
* App平台 修复 3.6.16 版引出的 Vue3 项目 vue 页面内联样式中 rpx 渲染错误的Bug [详情](https://ask.dcloud.net.cn/question/161256)
* 微信小程序平台 修复 3.6.16 版引出的 Vue2 项目部分情况下模板中使用多个逻辑表达式运行报错的Bug [详情](https://ask.dcloud.net.cn/question/161190)
### App插件(含5+App和uni-app的App端)
* Android平台 修复 3.6.11版引出的 使用 record 模块后 wgt 升级提示没有配置 record 模块的Bug [详情](https://ask.dcloud.net.cn/question/161167)
* Android平台 修复 3.6.16版引出的 部分设备沉浸式状态栏失效的Bug [详情](https://ask.dcloud.net.cn/question/161277)
* Android平台 修复 隐私政策提示框在未适配 disagreeMode 模式情况下仅显示一次的Bug [详情](https://uniapp.dcloud.net.cn/tutorial/app-disagreemode.html)

## 3.6.16.20230109-alpha
### HBuilder
* 修复 语言服务 uni-app Vue文件，script标签内，无法提示条件编译的Bug [详情](https://ask.dcloud.net.cn/question/159783)
* 修复 内置终端 绿柔主题下，选中终端文本，选中颜色没有显示的bug
* 优化 Markdown一键分享，网页所需的css资源和js资源，同步上传到uniCloud前端网页托管
* 修复 uni-app Vue3 运行到浏览器，浏览器Devtools控制台，日志路径显示错误的Bug
* 修复 uni-app 运行到iOS模拟器，开启uni调试，打开后调试窗体显示空白的Bug
* 修复 某些情况下 项目根目录.hbuilder/launch.json文件重复写入数据，频繁读写，导致编辑器卡顿的Bug
* 优化 原生App-云打包 Android打包 打包窗口不再显示`使用DCloud老版证书`（2022年11月30日以后创建的应用及以前未使用过老版本证书的应用不能再使用DCloud老版证书）
### uni-app插件
* App-Vue平台、Web平台 优化 input 组件支持 inputmode 属性 [详情](https://uniapp.dcloud.net.cn/component/input.html#inputmode)
* App平台 修复 Vue3 项目 nvue 页面 webview 组件 onPostMessage 事件无效的Bug [详情](https://ask.dcloud.net.cn/question/158925)
* App平台 修复 Vue3 项目 image 组件使用 base64 显示异常的Bug [详情](https://ask.dcloud.net.cn/question/158368)
* App-Android平台 修复 使用 tabbar 后页面多次跳转可能导致底部系统导航栏颜色变化的bug
* App-Android平台 修复 nvue 页面 live-pusher 组件拒绝相机权限后再手动开启，回到应用后可能无法调用相机预览的Bug [详情](https://ask.dcloud.net.cn/question/158518)
* App-iOS平台 修复 nvue 页面 ad-content-page 组件拉取广告配置失败后无法重新拉取的Bug
* App-iOS平台 修复 nvue 页面 map 组件使用自定义地图样式后切换卫星图无效的Bug [详情](https://ask.dcloud.net.cn/question/159316)
* App-iOS平台 修复 使用模拟器开启调试后启动应用白屏的Bug [详情](https://ask.dcloud.net.cn/question/160363)
* App-iOS平台 修复 Vue3 项目中 input 组件 disabled 无法动态修改的Bug [详情](https://ask.dcloud.net.cn/question/157958)
* Web平台、小程序平台 修复 uni-push2.0 WebSocket连接不稳定的Bug [详情](https://ask.dcloud.net.cn/question/159690)
* Web平台 修复 input 组件输入负数带出上次结果的Bug [详情](https://ask.dcloud.net.cn/question/159447)
* Web平台 修复 Vue3 项目 uni.navigateTo eventChannel 只会调用一次的Bug [详情](https://ask.dcloud.net.cn/question/155922)
* Web平台 修复 Vue3 项目 scroll-view 组件滚动频繁触发视图更新的Bug [详情](https://ask.dcloud.net.cn/question/149557)
* Web平台 修复 Vue3 项目 picker 组件 end 属性读取错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/4075)
* Web平台 修复 uni.setTabBarItem 导致 tab 切换生命周期异常的Bug [详情](https://ask.dcloud.net.cn/question/160739)
* 微信小程序平台 修复 Vue2 项目 模板中无法观测数组长度变化的Bug [详情](https://github.com/dcloudio/uni-app/issues/1827)
* 支付宝小程序平台 修复 Vue3 项目 使用内联样式运行报错的Bug [详情](https://ask.dcloud.net.cn/question/159362)
### uniCloud插件
* JQL语法 修复 使用 setUser 方法未传 permission 参数且使用触发器时报错的Bug
* JQL语法 修复 add 方法传递的字段值为对象且其中包含null值时报错的Bug
* JQL语法 新增 数据库触发器增加 triggerContext 参数，用于在 before 和 after 内共享数据 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#trigger-context)
* 阿里云 调整 正式版云存储单文件100MB限制调整为5GB
### App插件(含5+App和uni-app的App端)
* Android平台 更新 fastjson SDK为 1.2.83 版，解决安全检测可能报`Fastjson反序列化远程代码执行漏洞`的问题
* Android平台 更新 一键登录使用的个验SDK为 3.1.0.0 版，优化初始化和预登录速度
* Android平台 更新 UniPush 使用的个推核心组件SDK为 3.2.1.0 版；谷歌渠道个推 sdk-for-gj 为 4.4.3.1 版；解决发布到 Google Play 商店可能被下架的问题 [详情](https://ask.dcloud.net.cn/question/160249)
* Android平台 修复 3.6.12版引出的 从系统相册中选择文件在部分鸿蒙设备可能引起崩溃的Bug [详情](https://ask.dcloud.net.cn/question/159556)
* Android平台 修复 3.6.7版引出的 一键登录 登录完成后自动关闭登录界面，以及登录按钮 loading 动画效果缺失的Bug [详情](https://ask.dcloud.net.cn/question/159898)
* Android平台 修复 上架应用市场审核可能报`频繁自启动或关联启动第三方应用`的Bug [详情](https://ask.dcloud.net.cn/question/160965)
* Android平台 修复 设置 targetSdkVersion 值大于或等于 30 时使用高德地图引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/159801)
* Android平台 修复 连续多次调用 createBLEConnection 连接蓝牙设备，无法连接设备也可能触发成功回调的Bug [详情](https://ask.dcloud.net.cn/question/113070)
* Android平台 修复 上架OPPO应用市场可能提示`含数字天堂(dcloud)广告插件`的Bug [详情](https://ask.dcloud.net.cn/question/160501)
* iOS平台 更新 UniPush 使用的个推SDK为 2.7.2.0 版，因个推改为 Swift 版，需引入 Swift 库，可能导致打包后 ipa 文件变大 [详情](https://uniapp.dcloud.net.cn/tutorial/app-push-unipush.html#%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98)
* iOS平台 修复 设置应用语言为英文时部分系统界面可能会显示为回退语言的Bug [详情](https://ask.dcloud.net.cn/question/159445)
* iOS平台 修复 自定义基座真机运行可能导致 setStorage 保存的数据丢失的Bug [详情](https://ask.dcloud.net.cn/question/159903)
* iOS平台 修复 plus.nativeUI.toast 设置 style 为 inline 时 iconWidth/iconHeight 属性失效的Bug [详情](https://ask.dcloud.net.cn/question/160192)
* iOS平台 修复 uni-AD 优量汇开屏广告展示期间弹出提示框可能导致开屏界面不会关闭的Bug
* iOS平台 修复 startBluetoothDevicesDiscovery 搜索附近蓝牙设备返回数据没有 advertisData 字段的Bug [详情](https://ask.dcloud.net.cn/question/160178)

## 3.6.14.20221216-alpha
### HBuilder
* 修复 3.6.12版引出的 某些情况下，编辑器回车后，光标位置错误的Bug [详情](https://ask.dcloud.net.cn/question/159490)
* 修复 3.6.9版引出的 某些情况下，项目根目录生成了一个1.text测试文件的Bug [详情](https://ask.dcloud.net.cn/question/159580)
* 修复 3.6.7版引出的 html文件，运行到Chrome，启动了一个新的Chrome实例的Bug [详情](https://ask.dcloud.net.cn/question/159331)
* 修复 uni-app Web平台开启或停止浏览器Debug调试，某些情况下，控制台按钮重复显示的Bug
### uni-app插件
* App-Android平台 修复 使用 canvas 模块后 wgt 升级提示没有配置 canvas 模块的Bug [详情](https://ask.dcloud.net.cn/question/159283)
* App-iOS平台 修复 UniPush 2.0 在vue2项目中 启用离线推送后，调用 uni.getPushClientId 某些情况下获取不到cid的Bug [详情](https://ask.dcloud.net.cn/question/158921)
* 小程序平台 修复 3.6.11版引出的 使用 async/await 发布后运行报错的Bug [详情](https://ask.dcloud.net.cn/question/159413)
### uniCloud插件
* JQL语法 新增 触发器内可以获取用户信息和本次数据库操作结果 [用户信息](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#user-info)、[执行结果](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#result)
* JQL语法 新增 触发器内可以判断当前执行的语句是否和指定语句相同 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#is-equal-to-jql)
* JQL语法 调整 对于 schema 内定义的复杂类型数据（file、array、object）类型的字段，忽略赋给此字段的 null 值
* 本地调试插件 修复 在部分旧系统运行时本地调试服务启动失败的Bug [详情](https://ask.dcloud.net.cn/question/159343)
* 本地调试插件 修复 3.6.12版引出的 云函数 调试运行 无法进行Debug断点调试的Bug
* 本地调试插件 修复 阿里云正式版本地云函数内上传文件到云存储时，上传的文件无法在 uniCloud web 控制台看到的Bug [详情](https://ask.dcloud.net.cn/question/159109)
### App插件(含5+App和uni-app的App端)
* iOS平台 修复 plus.push.getClientInfoAsync 在应用热重启后调用不触发回调的Bug

## 3.6.12.20221207-alpha
* 修复 3.6.11引出的 uts文件 无法显示大纲视图的Bug
* 修复 3.6.11引出的 uts文件 右键菜单重排代码格式置灰的Bug
* 优化 App真机运行 设备选择窗口，标准基座和自定义基座，显示基座信息
* 优化 App真机运行 菜单【运行 - 运行到手机或模拟器】，移除菜单【运行基座选择】
* 【uniCloud插件】
  + 本地调试插件 修复 云函数调用云函数时，被调用云函数无返回值导致报错的Bug
* 【App插件(含5+App和uni-app的App端)】
  + iOS平台 修复 3.6.11 版本引出的 显示开屏广告时弹出系统 alert 窗偶现崩溃的Bug

## 3.6.11.20221205-alpha
* 新增 App真机运行 iOS设备选择窗口支持UDID显示和复制
* 新增 App真机运行 MacOSX uts插件 支持编译运行iOS标准基座到iOS真机设备
* 优化 App真机运行 iOS标准基座包体积，仅支持 arm64 架构。即不再支持iPhone 5S、iPad Air(mini2)以前的设备。此调整不影响打包和自定义基座。
* 修复 App真机运行 设备选择窗口 刷新设备列表 底部radio被改变的Bug
* 修复 App真机运行 uts插件 编译运行 某些情况下，Node进程没有结束的Bug
* 新增 uts插件 支持新建uts文件和平台目录
* 优化 uts插件 语言服务 提升代码提示速度，降低内存占用
* 优化 uts插件 热刷新速度，支持编译缓存，未修改不编译
* 修复 uts插件 语言服务 iOS平台 参数标签名称是关键字时报错的Bug
* 修复 语言服务 uni-app pages.json usingComponents拼写错误的Bug [详情](https://ask.dcloud.net.cn/question/158601)
* 修复 新建HBuilder窗口或者拖动标签卡创建新窗口，关闭该新窗口时会导致部分插件功能失效的Bug
* 优化 uniCloud db_init.json 初始化云数据库 当数据库表过多时，初始化云数据库超时的Bug
* 新增 App打包 控制台下载链接后的一键上传到uniCloud，支持上传到阿里云正式版云存储
* 修复 uni_modules插件 某些异常 package.json 缺少分类无法提交插件市场的Bug
* 【uni-app插件】
  + 新增 ad-interactive 互动广告组件 [详情](https://uniapp.dcloud.net.cn/component/ad-interactive.html)
  + App平台 新增 【ext api】 Wi-Fi 模块 [详情](https://uniapp.dcloud.net.cn/api/system/wifi.html)
  + App平台 优化 Vue2 项目 component is 支持传入组件选项和构造函数 [详情](https://ask.dcloud.net.cn/question/140044)
  + App平台 修复 nvue 页面 slider 组件某些情况下位置位置计算不准确的Bug [详情](https://ask.dcloud.net.cn/question/152714)
  + App-Android平台 修复 使用 tabbar 后页面多次跳转返回可能引起路由管理异常的Bug [详情](https://ask.dcloud.net.cn/question/158462)
  + App-Android平台 修复 3.6.9 版本引出的 uni.switchTab 在特殊场景可能无法正常切换页面的Bug [详情](https://ask.dcloud.net.cn/question/157720)
  + App-iOS平台 补齐 【ext api】 uni.onMemoryWarning [详情](https://ext.dcloud.net.cn/plugin?id=10071)
  + App-iOS平台 修复 3.6.7 版本引出的 ad 组件偶现加载优量汇广告成功但无法正常渲染的Bug
  + Web平台 修复 Vue3 项目 canvas 组件监听事件报错的Bug [详情](https://ask.dcloud.net.cn/question/158252)
  + 小程序平台 优化 vue3 项目使用 import 导入非 static 目录的资源生成后名称默认补充 hash [详情](https://github.com/dcloudio/uni-app/issues/4011)
  + 微信小程序平台 修复 Vue3 项目 v-for 循环事件可能错乱的Bug [详情](https://github.com/dcloudio/uni-app/issues/4015)
  + 微信小程序平台 修复 Vue3 项目 wxs 热更新失效的Bug [详情](https://ask.dcloud.net.cn/question/158252)
  + uni-im 全端支持Vue3 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-im.html)
  + uni-im 新增多媒体消息（含：语音、图片、视频、任意文件）和代码发送
  + uts插件 新增 在uts文件中可使用条件编译 //#ifdef APP-ANDROID 和 //#ifdef APP-IOS [详情](https://uniapp.dcloud.net.cn/tutorial/platform.html#uts-%E7%9A%84%E6%9D%A1%E4%BB%B6%E7%BC%96%E8%AF%91)
  + uts插件 App-Android平台 调整 内置库包名为`io.dcloud.uts`，类名为`UTSAndroid` [详情](https://uniapp.dcloud.net.cn/plugin/uts-for-android.html#iodcloudutsandroid)
  + uts插件 App-Android平台 优化 setTimeOut 函数线程池大小，支持多异步任务场景
  + uts插件 App-Android平台 修复 UTSJSONObject 构造函数无法传递复杂 JSON 参数的Bug
  + uts插件 App-Android平台 修复 UTSJSONObject 嵌套序列化存在冗余字段的Bug
  + uts插件 App-Android平台 修复 Array 索引不支持 number 类型的Bug
  + uts插件 App-Android平台 修复 JSON.stringify 参数为数组时返回字符串格式不正确的Bug
  + uts插件 App-iOS平台 新增 内置库`DCloudUTSFoundation` [详情](https://uniapp.dcloud.net.cn/plugin/uts-for-ios.html#dcloudutsfoundation)
  + uts插件 App-iOS平台 补齐 内置对象 Date、Number、Set、String、RegExp
  + uts插件 App-iOS平台 修复 console 打印对象在控制台输出格式不正确的Bug
  + hello uts 新增 系统API Alert 弹窗示例 [详情](https://ext.dcloud.net.cn/plugin?id=9892)
  + hello uts 补齐 iOS平台 三方SDK toast 消息提示框，监听设备位置变化示例 [详情](https://ext.dcloud.net.cn/plugin?id=9892)
* 【uniCloud插件】
  + 【重要】新增 数据库扩展js，{表名}.schema.ext.js，可实现数据库触发器。推荐用触发器替代action，更安全 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#trigger)
  + 【重要】uni-pay 2.0，从公共模块升级为包含前端页面、uni-pay-co云对象，让支付更加简单省心 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-pay.html)
  + JQL语法 修复 where 和 permission 内使用负数常量时报错的Bug [详情](https://ask.dcloud.net.cn/question/157993)
  + 本地调试插件 修复 调用 clientDB、jql扩展 时报找不到 action 的Bug [详情](https://ask.dcloud.net.cn/question/157997)
  + uniIdRouter 修复 vue3项目跳转时报错的Bug [详情](https://ask.dcloud.net.cn/question/158015)
  + 【重要】uni-id-co 新增 外部系统联登接口，可为外部系统创建与uni-id相对应的账号，使该账号可以使用依赖uniId的系统及功能 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#external)
  + uni-id-co 新增 设置密码接口 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#set-pwd)
  + uni-id-co 新增 URL化请求时鉴权签名验证 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#http-reqeust-auth)
  + uni-id-co 新增匹配到的用户不可在当前应用登录时的错误码 `uni-id-account-not-exists-in-current-app` [错误码说明](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#errcode)
  + uni-id-co 修复 微信登录时用户未设置头像的报错问题
  + uni-id-co 修复 无法从 clientInfo 中获取 uniIdToken
  + uni-id-pages 新增 登录后跳转设置密码页面配置项`setPasswordAfterLogin` [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#set-pwd-after-login)
  + uni-id-pages 新增 设置密码页面
  + uni-id-pages 优化 toast 错误提示时间为3秒
  + uni-admin 调整 群发短信功能的 schema 文件命名规范，将`batch-sms-template` `batch-sms-task` `batch-sms-result` 更改为 `opendb-sms-temlate` `opendb-sms-task` `opendb-sms-log` 以符合opendb规范
* 【App插件(含5+App和uni-app的App端)】
  + 【重要】调整 Camera&Gallery、Barcode、Orientation、Record等模块从引擎内置调整为独立模块，解决iOS平台隐私合规检测可能报包含麦克风、相机/相册、运动等权限的问题。云端打包默认不再包含以上模块，如需要请手动在 manifest.json -> 模块配置 中勾选[详情](https://uniapp.dcloud.net.cn/tutorial/app-modules.html#bcor)
  + Android平台 更新 UniPush 使用的个推SDK为 3.2.13.0 版，个推核心组件SDK为 3.1.12.0 版；谷歌渠道个推SDK为 4.10.1.0 版；解决隐私合规检测可能报超频采集的问题
  + iOS平台 更新 uni-AD 快手广告SDK为 3.3.33 版；快手内容联盟SDK为 3.3.32 版；今日头条穿山甲SDK为 4.9.0.5 版；穿山甲GroMore广告SDK为 3.8.0.2 版
  + iOS平台 修复 IAP支付 订单数据 orderInfo 参数异常时引起应用假死的Bug
  + iOS平台 修复 3.6.10版本引出的 三方登录授权不触发回调的Bug [详情](https://ask.dcloud.net.cn/question/158380)

## 3.6.10.20221121-alpha
* 修复 3.6.9引出的 uni-app CLI项目，当存在uts插件时，无法正常编译和运行的Bug
* 修复 uni-app uts插件 语言服务 `import x from '@/uni_modules/'` uts插件路径提示错误的Bug
* 修复 App真机运行 设备选择窗口 某些情况下，点击运行按钮，HBuilderX出现崩溃的Bug
* 优化 uts插件 iOS平台 本地编译和真机运行速度
* 【uni-app插件】
  + App平台 修复 Vue2 项目 编辑 uts 插件代码热更新失效的Bug
  + App平台 修复 Vue2 项目 nvue 页面不支持 uts 插件的Bug [详情](https://ask.dcloud.net.cn/question/157435)
  + App平台 修复 darkmode 模式下设置 statusBar 颜色不正常的Bug
  + App平台 修复 nvue 首页设置 navigationBarTextStyle 无效的Bug [详情](https://ask.dcloud.net.cn/question/150485)
  + App平台 修复 uni.startSoterAuthentication（生物识别）识别错误时 loading 没有文字提示的Bug [详情](https://ask.dcloud.net.cn/question/157353)
  + App-Android平台 修复 uni.request 不支持 head 请求的Bug [详情](https://ask.dcloud.net.cn/question/136717)
  + App-Android平台 修复 页面中存在多个 input 组件时获取焦点光标位置可能不正确的Bug
  + App-Android平台 修复 nvue live-pusher 组件在 Android11+ 设备使用移动网络无法预览的Bug [详情](https://ask.dcloud.net.cn/question/156532)
  + App-Android平台 调整 uts插件 Date.getDay 从以周日为1统一调整为周日为0
  + App-Android平台 修复 uts插件 不支持函数参数为数组的Bug
  + App-Android平台 修复 uts插件 JSON.parse 不支持 JSONArray 的Bug
  + Web平台 修复 Vue3 项目 --window-top 计算错误的Bug [详情](https://ask.dcloud.net.cn/question/157164)
  + Web平台 修复 Vue3 项目配置全局 loading、error 组件无效的Bug [详情](https://ask.dcloud.net.cn/question/157122)
  + 支付宝小程序平台 修复 page-meta 组件 root-font-size 属性无效的Bug [详情](https://ask.dcloud.net.cn/question/157168)
  + uni-im 支持 非uniCloud 或 不基于uni-id-pages 开发的项目 接入 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-im.html)
* 【uniCloud插件】
  + 【重要】阿里云商用版正式上线 [详情](https://ask.dcloud.net.cn/article/40144)
  + JQL语法 新增 支持 geoNear 以实现地理位置查询 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql.html#geo-near)
  + JQL语法 修复 部分有权限进行的查询被误报权限校验未通过的Bug
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 新增 隐私政策提示框支持 showAlways 配置是否每次启动都弹窗提示 [详情](https://uniapp.dcloud.net.cn/tutorial/app-privacy-android.html)
  + Android平台 修复 监听系统暗黑模式主题切换事件可能无效的Bug [详情](https://ask.dcloud.net.cn/question/157497)
  + Android平台 修复 云端打包 使用自有证书可能报 `Invalid keystore format` 错误的Bug [详情](https://ask.dcloud.net.cn/question/157057)
  + Android平台 修复 云端打包 配置应用清单文件 AndroidManifest.xml 的 package 属性值与包名相同时打包失败的Bug
  + iOS平台 修复 3.6.7版本引出的 设置启动页不自动关闭无效的Bug [详情](https://ask.dcloud.net.cn/question/157721)
  + iOS平台 修复 plus.screen.lockOrientation、plus.screen.unlockOrientation 在 iOS16 设备无效的Bug [详情](https://ask.dcloud.net.cn/question/155357)
  + iOS平台 修复 播放音频时无法正常录音的Bug [详情](https://ask.dcloud.net.cn/question/157408)
  + iOS平台 修复 设置暗黑模式跟随系统主题可能无效的Bug
* 【uni小程序SDK】
  + Android平台 修复 默认包含设置角标权限的Bug

## 3.6.9.20221114-alpha
* 【重要】App真机运行 iOS标准基座 支持使用Apple证书签名，签名后可运行标准基座到iOS真机设备（需mac电脑） [详情](https://uniapp.dcloud.net.cn/tutorial/run/ios-apple-certificate-signature.html)
* 新增 MarkDown 支持 Mermaid图，包含流程图 [详情](https://hx.dcloud.net.cn/Tutorial/Language/markdown?id=mermaid)
* 新增 MarkDown 文件和图片语法`![]()`、`[]()`中，支持提示文件路径 [详情](https://hx.dcloud.net.cn/Tutorial/Language/markdown?id=PathHints)
* 新增 MarkDown 代码区 kotlin 、 uts 等语言支持代码高亮
* 修复 代码助手 存在某些不支持的图片格式时，图片预览失效的Bug
* 新增 uts插件 iOS平台 支持本地编译和真机运行，需要配置Xcode环境 [详情](https://uniapp.dcloud.net.cn/tutorial/run/uts-development-ios.html)
* 新增 uts插件 Android平台 真机运行支持三方 Gradle 仓储 [详情](https://uniapp.dcloud.net.cn/tutorial/run/uts-development-android.html)
* 优化 uts插件 语言服务 支持iOS系统API、Android系统API的代码提示
* 优化 uts插件 语言服务 Android平台 完善R资源的代码提示
* 优化 uts插件 语言服务 Android平台 支持免导入使用java.lang.*下的类
* 修复 MacOSX 格式化ts文件，首行代码格式化后被添加空格的Bug
* 修复 HBuilderX 非正常退出时，语言服务进程没有退出的Bug
* 修复 windows 某些型号的电脑，HBuilderX 拖动内置浏览器边框后闪退的Bug
* 修复 App真机运行 设备选择窗口，某些情况下，错误提示弹窗显示到设备选择窗口后面，导致HBuilderX无法进行任何操作的Bug
* 修复 App真机运行 iOS离线SDK制作自定义基座，target不是HBuilder时，同步文件失败的Bug
* 【uni-app插件】
  + 新增 uni错误规范 [详情](https://uniapp.dcloud.net.cn/tutorial/err-spec.html)
  + App、Web平台 新增 暗黑模式（DarkMode） [详情](https://uniapp.dcloud.net.cn/tutorial/darkmode.html)
  + App、Web平台 修复 radio 组件禁用状态样式异常的Bug
  + App平台 新增 nvue 页面 MapContext 支持 setLocMarkerIcon 方法 [详情](https://uniapp.dcloud.net.cn/api/location/map.html#setLocMarkerIcon)
  + App平台 新增 nvue list 组件支持 render-reverse 属性 [详情](https://uniapp.dcloud.net.cn/component/list.html#%E5%B1%9E%E6%80%A7)
  + App平台 修复 Vue2 项目使用组合式 API 时 onReady 声明周期 template ref 未绑定的Bug
  + App平台 修复 Vue3 项目 template ref 会被代理的Bug
  + App平台 修复 Vue3 项目设置导航栏背景色为 rgba 色值无效的Bug [详情](https://ask.dcloud.net.cn/question/135111)
  + App平台 修复 Vue3 项目根节点 height:100% 无效的Bug [详情](https://ask.dcloud.net.cn/question/156564)
  + App-Android平台 新增 【ext api】 uni.onMemoryWarning [详情](https://ext.dcloud.net.cn/plugin?id=10071)
  + App-Android平台 新增 uts插件 生命周期函数 on/offAppTrimMemory、on/offAppConfigChange 等 [详情](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html#iodcloudutsandroid)
  + App-Android平台 修复 uts插件 libs 包含三方 aar 时，丢失部分 jar 包的Bug
  + App-Android平台 修复 uts插件 无法继承内部类的Bug
  + App-iOS平台 修复 Vue3 项目录音播放无效的Bug [详情](https://ask.dcloud.net.cn/question/155741)
  + App-iOS平台 修复 uts插件 类构造函数无法使用外参的Bug
  + 微信小程序平台 修复 3.6.8 版本引出的 Vue3 项目在 vite.config.js 内定义编译注入的全局常量导致使用了 uniCloud 的客户端报错的Bug
  + 支付宝小程序平台 修复 uni.showLoading 提示 mask 参数无效的Bug [详情](https://ask.dcloud.net.cn/question/156944)
  + 支付宝小程序平台 修复 Vue3 项目 eventChannel 通信失败的Bug [详情](https://github.com/dcloudio/uni-app/issues/3945)
  + 字节跳动小程序平台 优化 默认启用 component2 [详情](https://ask.dcloud.net.cn/question/156550)
  + hello uts 新增 Android平台获取用户输入、播放asset音频、调用系统拍照示例 [详情](https://ext.dcloud.net.cn/plugin?id=9892)
* 【uniCloud插件】
  + 【重要】新增 uni-im 云端一体的、全平台的、免费的、开源即时通讯系统 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-im.html)
  + jql语法 修复 使用 add 数据库运算方法报错的Bug [详情](https://ask.dcloud.net.cn/question/156261)
  + jql语法 修复 使用部分 js 关键字导致查询条件或 field 报错的Bug
  + jql语法 修复 使用 getTemp 联表查询时，如果主表关联字段在 schema 内为数组类型但实际数据无此字段时报错的Bug
  + 云对象 新增 url 化支持通过多段 path 路径调用方法，以第一段作为云对象方法名 [详情](https://uniapp.dcloud.net.cn/uniCloud/http.html#request-co-url)
  + 本地调试插件 修复 HBuilderX 3.6.7 引出的断点进入nodejs内置模块的Bug
  + 安全网络 调整 统一错误码规范 [详情](https://uniapp.dcloud.net.cn/uniCloud/secure-network.html#err-code)
  + uni-id 升级密码加密算法，支持hmac-sha256加密 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#password-safe)
  + uni-id 新增 开发者可以自定义密码加密规则 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#custom-password-encrypt)
  + uni-id 新增 支持将其他系统用户迁移至uni-id [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#move-users-to-uni-id)
  + uni-id 支持URL化方式请求 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#adapter-http)
* 【App插件(含5+App和uni-app的App端)】
  + 新增 Stripe支付支持设置账单信息 [详情](https://uniapp.dcloud.net.cn/tutorial/app-payment-stripe.html)
  + Android平台 新增 支持暗黑模式 [详情](https://ask.dcloud.net.cn/article/36995)
  + Android平台 更新 uni-AD 今日头条穿山甲广告SDK 为 4.9.0.8 版；穿山甲GroMore广告SDK 为 4.8.0.0 版；腾讯优量汇广告SDK 为 4.492.1362 版
  + Android平台 更新 高德地图SDK为 9.5.0 版，高德定位SDK为 6.1.0 版，解决隐私合规检测可能报高德SDK收取MAC地址、ANDROID ID的问题 [详情](https://ask.dcloud.net.cn/question/154268)
  + Android平台 修复 3.6.7版本引出的 应用后台切前台插屏广告可能不显示的Bug
  + Android平台 修复 视频播放控件 VideoPlayer 隐私合规检测可能报`数字天堂SDK获取传感器`的Bug [详情](https://ask.dcloud.net.cn/question/156360)
  + Android平台 修复 原生隐私政策提示框在部分设备 message 内容可能显示不正常的Bug [详情](https://ask.dcloud.net.cn/question/156445)
  + iOS平台 修复 3.6.0版本引出的 开屏广告自定义底部图片、背景色不生效的Bug
  + iOS平台 修复 标题栏 titleNView 设置默认导航栏颜色可能导致与状态栏颜色不一致的Bug
  + iOS平台 修复 setUIStyle 设置暗黑模式可能无效的Bug

## 3.6.8.20221027-alpha
* 修复 App真机运行 打开Object类型的日志后，内容没有格式化的Bug
* 修复 uni_modules 插件市场导入插件，运行缓慢超时导致提示`插件处理外部应用请求未能完成`的Bug
* 【uni-app插件】
  + 【重要】新增 vue2 项目支持开发、使用 uts 插件 [详情](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html)
  + 新增 Vue2 项目支持使用组合式 API [详情](https://uniapp.dcloud.net.cn/tutorial/vue-composition-api.html)
  + 修复 3.6.7 版本引出的 Vue3 项目使用 TypeScript 后部分对象无法访问的Bug [详情](https://github.com/dcloudio/uni-app/issues/3930)
  + App平台、Web平台 新增 地理位置更新相关接口 [详情](https://uniapp.dcloud.net.cn/api/location/location-change.html)
  + App平台 修复 3.6.7 版本引出 Vue3 项目的 nvue 页面全局样式无效的Bug [详情](https://ask.dcloud.net.cn/question/155639)
  + App平台 修复 Vue2 项目移除页面根节点后导致事件异常的Bug [详情](https://ask.dcloud.net.cn/question/155057)
  + App平台 修复 Vue2 项目列表不使用 index 作为 key 时更新数据导致事件异常的Bug [详情](https://ask.dcloud.net.cn/question/155238)
  + App-Android平台 优化 Vue3 项目 minUserAgentVersion 默认配置为 49，避免低版本webview上白屏无提示 [详情](https://uniapp.dcloud.net.cn/collocation/manifest.html#appwebview)
  + App-Android平台 修复 uni.getStorageSync在某些情况下可能报`SyntaxError`错误的Bug [详情](https://ask.dcloud.net.cn/question/154284)
  + App-Android平台 新增 uts插件 支持application/activity部分生命周期函数 [详情](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html#iodcloudutsandroid)
  + App-Android平台 修复 uts插件 不支持泛型通配符语法的Bug [详情](https://ask.dcloud.net.cn/question/155942)
  + App-iOS平台 修复 在 iOS16 设备 nvue 页面关闭、开启下拉刷新效果时偶现崩溃的Bug
  + App-iOS平台 修复 3.6.0版本引出的 nvue list 组件内使用 ad 信息流广告组件偶发渲染空白的Bug [详情](https://ask.dcloud.net.cn/question/155752)
  + Web平台 修复 Vue2 项目中 css 媒体查询中使用 page 选择器不生效的Bug
  + 【重要】微信小程序平台 新增 uni-AD 安全激励视频，提供防刷的服务器回调 [详情](https://uniapp.dcloud.net.cn/component/ad-weixin.html)
  + 支付宝小程序 新增 uni.onKeyboardHeightChange 监听键盘高度变化 [详情](https://uniapp.dcloud.net.cn/api/key.html#onkeyboardheightchange)
  + 支付宝小程序 修复 小程序组件中的事件触发时机较早时在 Vue 组件中无法监听的Bug
* 【uniCloud插件】
  + 【重要】新增 安全网络 客户端校验功能，防止伪造的客户端请求服务器 [详情](https://uniapp.dcloud.net.cn/uniCloud/secure-network.html#verify-client)
  + 新增 `uni-clear-temp-data` 插件，用于自动清理数据库中的过期数据 [详情](https://ext.dcloud.net.cn/plugin?id=9826)
  + 修复 HBuilderX插件 `uni-`开头的 schema 文件 右键菜单缺少【opendb检查更新】的Bug
  + 修复 HBuilderX插件 本地云函数调用 redis 接口传较大的数据时报错的Bug [详情](https://ask.dcloud.net.cn/question/155804)
  + 修复 uniIdRouter 使用相对路径跳转时附带的 uniIdRedirectUrl 参数错误的Bug [详情](https://ask.dcloud.net.cn/question/155904)
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 修复 chooseVideo 使用相机拍摄视频在Android10及以上设备可能失败的Bug [详情](https://ask.dcloud.net.cn/question/155877)
  + Android平台 修复 chooseImage、chooseVideo 存在读取设备应用安装列表的行为可能导致隐私检测不合规的Bug
  + Android平台 修复 应用安全检测可能报`app关联启动`的Bug
  + Android平台 修复 3.6.0版本引出的 首次真机运行隐私政策提示框可能不弹出的Bug
  + iOS平台 更新 uni-AD 百度百青藤广告SDK 为 4.901 版；快手广告SDK 为 3.3.32 版
  + iOS平台 更新 微信SDK 为 1.9.6 版
  + iOS平台 修复 分享到微信收藏夹时跳转到朋友圈的Bug [详情](https://ask.dcloud.net.cn/question/155362)

## 3.6.7.20221018-alpha
* 【重要】升级 HBuilderX 内置Node版本升级为16.17.0，内置npm版本升级为6.14.12
* 优化 Git插件 git pull操作 状态栏消息增加查看日志功能 方便查看日志
* 调整 设置 将语言服务相关的配置聚合到`语言服务配置`配置项中
* 新增 Node调试 支持附加(attach)到已经启动的node进程上断点调试 [详情](https://hx.dcloud.net.cn/Tutorial/extension/node-development?id=attach)
* 优化 Windows 当Node进程被安全软件拦截，导致语言服务等Node插件启动失败时，弹窗提示
* 修复 代码助手 代码助手显示后，拖动到编辑器底部，任意光标位置回车后，中间代码丢失的Bug
* 修复 代码助手 当快速输入代码块时，某些情况下，代码提示窗口右侧信息显示其它语言服务返回结果的Bug
* 修复 代码助手 CSS class存在多个时，快速敲空格然后按左键，导致代码提示回车后替换位置错误的Bug
* 修复 代码助手 CSS 大文件代码提示速度过慢的Bug
* 修复 语法校验 uni-app项目(非CLI) 当项目下存在tsconfig.json时，某些情况下，语法校验误报的Bug
* 修复 语法校验 JSON 文件末尾存在中文`，`时，报错波浪线不显示的Bug
* 修复 转到定义 uni-app App.vue style引入多个文件, class转到定义只对最后一个文件生效的Bug [详情](https://ask.dcloud.net.cn/question/154824)
* 修复 语言服务 某些情况下，语言服务频繁报错崩溃，HBuilderX窗口右下角频繁弹窗报错的Bug
* 修复 内置浏览器 Windows 某些情况下，拖动内置浏览器，HBuilderX闪退的Bug
* 修复 App真机运行 3.5.5引出的 uni-app 运行到iOS模拟器，修改nvue文件，无法同步修改的Bug
* 修复 App真机运行 3.5.5引出的 5+app 运行到iOS 某些情况下，日志没有打印的Bug
* 优化 uni-app 运行到Web 支持选择使用Chrome Debug、使用内置浏览器Debug（控制台点击虫子图标，可弹出选择菜单）
* 修复 uni-app 运行到内置浏览器 某些情况下，Cookie不一致的Bug
* 新增 uni-app manifest.json 可视化界面App模块配置 增加"安全网络" [详情](https://uniapp.dcloud.net.cn/uniCloud/secure-network.html)
* 修复 uniCloud 前端网页托管 某些情况下，发布失败，仍然执行上传操作的Bug
* 新增 uni_modules 支持配置模块的初始化脚本。可用于定时任务设置随机开始时间 [详情](https://uniapp.dcloud.net.cn/plugin/uni_modules.html#package-json)
* 修复 uni-app 真机运行 uts Android版插件调用内置依赖库中的API时需要手动下载并添加到lib目录的Bug [详情](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html#tempnotice)
* 【uni-app插件】
  + 【重要】新增 uts iOS版插件。将uts代码转为swift代码。 [详情](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html)
  + 【重要】新增 `uni ext api`。将不常用的API剥离为uni_modules插件，但仍使用uni.开头的API。[详情](https://uniapp.dcloud.net.cn/api/extapi.html)
  + 【重要】App-Android平台 修复 getSystemInfo 的 deviceId 属性偶尔获取失败和多设备获取重复的Bug（注意此修改造成的向下兼容问题）[详情](https://uniapp.dcloud.net.cn/api/system/info.html)
  + vue3 项目 vite 依赖版本升级至最新 3.1.8
  + App平台、Web平台 新增 【ext api】 uni.getBatteryInfo [详情](https://uniapp.dcloud.net.cn/api/system/batteryInfo.html)
  + App平台、Web平台 修复 picker 组件日期类型无法使用超出默认的年份范围值的Bug [详情](https://ask.dcloud.net.cn/question/131332)
  + App平台、Web平台 修复 iOS16 系统 input 组件 type=digit 无法输入小数点的Bug [详情](https://ask.dcloud.net.cn/question/154584)
  + App平台、Web平台 修复 editor 组件 insertImage 触发 input 事件没有 alt 属性的Bug [详情](https://ask.dcloud.net.cn/question/155163)
  + App平台、Web平台 修复 vue3 项目 editor 组件重新加载获取不到 EditorContext 的Bug [详情](https://ask.dcloud.net.cn/question/154702)
  + App平台 新增 nvue 页面 picker-view 组件增加 mask-top-style、mask-bottom-style 属性 [详情](https://uniapp.dcloud.net.cn/component/picker-view.html)
  + App平台 优化 video 组件支持 title 属性 [详情](https://uniapp.dcloud.net.cn/component/video.html)
  + App平台 修复 hover-class 属性不支持多个 class 的Bug [详情](https://ask.dcloud.net.cn/question/152506)
  + App平台 修复 vue3 项目 uts 插件 export default class 不生效的Bug [详情](https://ask.dcloud.net.cn/question/154164)
  + App平台 修复 vue3 项目 v-for 可能渲染失败的Bug [详情](https://ask.dcloud.net.cn/question/154836)
  + App平台 修复 vue3 项目 tabbar.broderStyle 自定义色值无效的Bug [详情](https://ask.dcloud.net.cn/question/150718)
  + App平台 修复 vue3 项目 nvue 页面 switch 组件 disabled 属性无效的Bug [详情](https://ask.dcloud.net.cn/question/154577)
  + App-Android平台 修复 3.5.5版本引出 input 组件自动获取焦点可能失效的Bug [详情](https://ask.dcloud.net.cn/question/153481)
  + App-iOS平台 修复 nvue swiper 组件使用 rpx 时在部分设备可能无法正常滑动切换的Bug [详情](https://ask.dcloud.net.cn/question/149260)
  + Web平台 优化 uni.previewImage 在 PC 端增加切换和关闭按钮
  + Web平台 修复 tabbar 某些情况下显示重复的 badge 的Bug [详情](https://ask.dcloud.net.cn/question/153336)
  + Web平台 修复 uni.openLocation 导航未自动获取当前位置Bug [详情](https://ask.dcloud.net.cn/question/155066)
  + Web平台 修复 vue3 项目 titleNView 中 buttons 的 select 为 true 时图标不显示的Bug [详情](https://ask.dcloud.net.cn/question/153179)
  + Web平台 修复 vue3 项目 进入 tabbar 重复触发 onLoad 的 Bug [详情](https://ask.dcloud.net.cn/question/154066)
  + web平台 修复 vue3 项目 CSS 中的 v-bind 使用 rpx 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3884)
  + 小程序平台 修复 改变数据时 setData 调用异常的Bug [详情](https://github.com/dcloudio/uni-app/issues/3787)
  + 小程序平台 修复 vue3 项目 CSS 中的 v-bind 使用非 setup 中的数据不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3887)
  + 小程序平台 修复 vue3 项目 作用域插槽嵌套使用时可能渲染错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/3886)
  + 小程序平台 修复 vue3 项目 作用域插槽静态数据渲染错误的Bug [详情](https://ask.dcloud.net.cn/question/153150)
  + 小程序平台 修复 vue3 项目 v-for 里的插槽可能渲染错误的Bug [详情](https://ask.dcloud.net.cn/question/155008)
  + 小程序平台 修复 vue3 项目 发行为混合分包，页面返回可能报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3923)
  + 微信小程序平台 修复 vue3 项目 scroll-view 的 drag 相关事件不触发的Bug [详情](https://github.com/dcloudio/uni-app/issues/3921)
  + 微信小程序平台 修复 vue3 项目 uni://form-field 不生效的Bug [详情](https://ask.dcloud.net.cn/question/155373)
  + 百度小程序平台 修复 uni.createIntersectionObserver 无法监听多个节点的Bug [详情](https://github.com/dcloudio/uni-app/issues/3835)
  + 百度小程序平台 修复 node_modules 目录中的静态资源生成目录错误的Bug [详情](https://ask.dcloud.net.cn/question/154595)
  + 百度小程序平台 修复 onInit 生命周期不触发的Bug [详情](https://ask.dcloud.net.cn/question/154352)
  + 百度小程序平台 修复 vue2 项目 使用 usingSwanComponents 配置动态库组件内事件无法获取参数的Bug [详情](https://ask.dcloud.net.cn/question/155281)
  + 百度小程序平台 修复 vue3 项目 不能正常使用动态库组件的Bug [详情](https://github.com/dcloudio/uni-app/issues/3864)
  + 支付宝小程序平台 修复 编译成小程序插件后 uni.hideLoading 等接口无法访问的Bug [详情](https://github.com/dcloudio/uni-app/issues/2974)
  + 支付宝小程序平台 修复 page-container 组件被当作自定义组件编译的Bug [详情](https://ask.dcloud.net.cn/question/154028)
  + 支付宝小程序平台 修复 uni.showToast 不支持 duration 参数的Bug [详情](https://ask.dcloud.net.cn/question/147279)
  + 支付宝小程序平台 修复 小程序插件内的组件未使用事件运行报错的Bug [详情](https://github.com/dcloudio/uni-app/pull/3903)
  + QQ小程序平台 修复 vue3 项目 uni.createCanvasContext 传入 this 报错的Bug [详情](https://ask.dcloud.net.cn/question/154223)
  + 字节跳动小程序平台 新增 支持使用小程序插件 [详情](https://github.com/dcloudio/uni-app/issues/3917)
  + 字节跳动小程序平台 修复 vue3 项目使用小程序自定义组件可能报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3915)
  + 快手小程序平台 新增 页面支持分包 [详情](https://uniapp.dcloud.net.cn/collocation/pages.html#subpackages)
  + 快手小程序平台 优化 uni.requestPayment 实现改用 ks.pay [详情](https://ask.dcloud.net.cn/question/152948)
  + uni统计 修复 3.4.9版本引出的 deviceId 获取方式变化，导致 uni统计2.0 App-Android 平台部分统计数据不准确的Bug [详情](https://ask.dcloud.net.cn/article/40097)
* 【uniCloud插件】
  + 【重要】新增 `安全网络` uni-app客户端和unicloud实现安全通讯，验证客户端身份和加密数据，防刷利器 [详情](https://uniapp.dcloud.net.cn/uniCloud/secure-network.html)
  + 新增 客户端sdk 新增 uniCloud.databaseForJQL 接口，拉齐在云函数中的写法。相比之前 database，返回值移除了多一层的 result [详情](https://uniapp.dcloud.net.cn/uniCloud/clientdb.html#jssdk)
  + 新增 客户端sdk uniCloud.importObject增加 parseSystemError 选项，用于处理云对象未捕获的错误或客户端网络错误，以便给用户展示友好的错误信息 [详情](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#auto-ui)
  + 修复 本地调试插件 连接本地云函数 require 出错时仅第一次报出错误的Bug
  + uni-id-co 新增 支持微信授权手机号登录方式 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#login-by-weixin-mobile)
  + uni-id-co 新增 解绑第三方平台账号 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#unbind-third-account)
  + uni-id-co 新增 微信绑定手机号支持通过`getPhoneNumber`事件回调的`code`绑定 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#bind-mobile-by-mp-weixin)
  + uni-admin 新增 群发短信功能 [详情](https://uniapp.dcloud.net.cn//uniCloud/admin.html#群发短信)
  + uni-admin 修复 uni统计 App-Android 平台部分统计数据不准确的Bug [详情](https://ask.dcloud.net.cn/article/40097)
  + uni-admin 修复 uni统计 周/月数据不准确的Bug
* 【App插件(含5+App和uni-app的App端)】
  + 更新 uni-AD 腾讯优量汇SDK iOS为 4.13.90 版；快手广告SDK Android为3.3.32，iOS为 3.3.31 版；快手内容联盟SDK iOS为 3.3.31 版；今日头条穿山甲SDK iOS为 4.8.0.3 版；穿山甲GroMore广告SDK iOS为 3.7.0.0 版；Sigmob广告联盟SDK Android为 4.7.0 版，iOS为 4.5.0 版；百度百青藤广告SDK Android为 9.241 版；华为广告SDK Android为 13.4.56.302 版
  + 【重要】Android平台 修复 plus.device.uuid 在高版本Android上不同设备获取的值可能相同的Bug。如之前依赖uuid，需注意处理兼容
  + 新增 plus.device.getDeviceId 获取匿名设备标识 [详情](https://www.html5plus.org/doc/zh_cn/device.html#plus.device.getDeviceId)
  + Android平台 新增 模板隐私政策提示框支持配置`游客模式`按钮 [详情](https://uniapp.dcloud.net.cn/tutorial/app-privacy-android.html)
  + Android平台 更新 Paypal SDK 为 0.6.2 版，解决设置targetSdkVersion为31打包失败的问题 [详情](https://ask.dcloud.net.cn/question/154976)
  + Android平台 修复 UniPush 异步获取推送标识在部分情况可能返回慢的Bug
  + Android平台 修复 应用设置仅支持竖屏时在部分Android8设备可能引起应用崩溃的Bug
  + Android平台 修复 X5 内核在部分情况无法正确加载的Bug [详情](https://ask.dcloud.net.cn/question/152854)
  + Android平台 修复 直播推流 LivePusher 在部分场景可能引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/147593)
  + Android平台 修复 视频播放控件 VideoPlayer 切换视频资源后静音状态可能失效的Bug [详情](https://ask.dcloud.net.cn/question/153257)
  + Android平台 修复 视频播放控件 VideoPlayer 销毁时可能导致卡顿的Bug [详情](https://ask.dcloud.net.cn/question/153483)
  + Android平台 修复 视频播放控件 VideoPlayer 在部分情况下标题栏不显示的Bug
  + Android平台 修复 chooseVideo 选择视频文件在鸿蒙系统可能无法加载缩略图的Bug [详情](https://ask.dcloud.net.cn/question/152527)
  + Android平台 修复 一键登录 全屏模式设置背景图时沉浸式效果不正确的Bug
  + Android平台 修复 上架应用市场审核可能报`数字天堂SDK获取传感器的行为`的Bug [详情](https://ask.dcloud.net.cn/question/155043)
  + Android平台 修复 本地打包生成的自定义基座可能无法识别安装的Bug
  + Android平台 修复 3.6.0版本引出的 在 Android4.4 设备无法正常运行的Bug [详情](https://ask.dcloud.net.cn/question/153910)
  + 【重要】iOS平台 新增 云端打包支持原生应用配置文件 Info.plist 和资源目录 Resources [详情](https://uniapp.dcloud.net.cn/tutorial/app-nativeresource-ios)
  + iOS平台 修复 使用`阿里百川电商`SDK 5.x版，云端打包报符号冲突错误的Bug [详情](https://ask.dcloud.net.cn/question/153138)
  + iOS平台 修复 视频播放控件 VideoPlayer 标题栏、进度条样式不正确的Bug [详情](https://ask.dcloud.net.cn/question/153945)
  + iOS平台 修复 uni-AD 穿山甲Gromore 激励视频偶现可能无法显示的Bug [详情](https://ask.dcloud.net.cn/question/153717)
  + iOS平台 修复 3.6.0版本引出的 uni原生语言插件Hook不到applicationWillEnterForeground、applicationDidEnterBackground等系统事件的Bug
  + iOS平台 修复 安全检测可能报获取设备idfv的Bug

## 3.6.3.20220919-alpha
* 修复 3.6.1引出的 HBuilderX 关闭标签卡，某些情况下出现闪退的Bug [详情](https://ask.dcloud.net.cn/question/153398)
* 修复 3.6.1引出的 Windows 内置浏览器 手机设备模式 无法选择元素的Bug
* 修复 HBuilderX 代码提示过程中切换到其它程序，某些情况下，代码提示窗口会覆盖在其它程序上面的Bug
* 修复 3.6.1引出的 语言服务 uni-app CLI项目 px转rpx失效的Bug [详情](https://ask.dcloud.net.cn/question/153384)
* 修复 3.6.1引出的 控制台日志 某些类型的日志输出错误的Bug
* 修复 uni-app 运行到iOS模拟器，控制台日志被截断或输出不全的Bug
* 修复 uni-app 运行到Android模拟器，Windows上某些Android模拟器运行失败的Bug
* 修复 uni-app 运行到Android，某些情况下，控制台提示编译成功后，没有反应的Bug
* 修复 App安心打包 Android 新版支付宝SDK引出的，安心打包失败的Bug
* 【uni-app插件】
  + 小程序平台 修复 onReady 生命周期触发两次的Bug [详情](https://ask.dcloud.net.cn/question/153422)

## 3.6.1.20220907-alpha
* 修复 3.6.0引出的 Windows 内置浏览器 网络请求无法跨域的Bug [详情](https://ask.dcloud.net.cn/question/152510)
* 修复 3.6.0引出的 Windows 内置浏览器 某些情况下，浏览器背景色错误的Bug [详情](https://ask.dcloud.net.cn/question/152647)
* 修复 编辑器 关闭选项卡 某些情况下，没有记忆折叠状态的Bug
* 修复 语言服务 JavaScript `Object.`不提示es6+新增方法的Bug
* 修复 语言服务 uni-app pages.json文件, page字段路径提示回车后补全错误的Bug
* 修复 语言服务 uni-app nvue文件 css class 转到定义失败的Bug [详情](https://ask.dcloud.net.cn/question/152522)
* 修复 语言服务 uni-app nvue文件 script和style标签 无法提示lang属性的Bug
* 修复 语言服务 Vue文件 stylus代码没有提示的Bug
* 修复 语言服务 `import xxx from 'XXX.vue'` 当不带vue后缀，提示模块找不到，以及无法转到定义的Bug
* 修复 语言服务 jsx和tsx文件 敲字符`.`时无法自动触发代码提示的Bug
* 新增 语言服务 内置语法校验 支持warning级别
* 修复 语言服务 启用JavaScript校验 在Vue文件 Script节点不生效的Bug
* 修复 语言服务 html文件 关闭JavaScript校验功能配置后，错误红色波浪线仍然存在的Bug
* 修复 语言服务 多行错误时，鼠标悬浮在非第一行，错误提示不显示的Bug
* 修复 App-云打包 某些情况下 项目下单个静态资源文件过大(比如超过100M)时 无法提交打包的Bug
* 修复 App-云打包 Windows 某些情况下，提交打包，HBuilderX出现闪退的Bug
* 修复 uniCloud 云函数 当云函数依赖第三方库，上传并运行，执行失败的Bug
* 【uni-app插件】
  + App平台 修复 vue3 项目切换 tabbar 页面时调用 uni.createVideoContext 的 pause 无法暂停播放的Bug[详情](https://ask.dcloud.net.cn/question/151933)
  + App-Android平台 修复 uts 插件 部分情况下编译后丢失导入类的Bug [详情](https://ask.dcloud.net.cn/question/152597)
  + App-Android平台 修复 uts 插件 定义类型时使用 kotlin 基础类型（如 Int）时，编译报错的Bug
  + App-Android平台 修复 uts 插件 云打包时未包含 AndroidManifest.xml 的Bug
  + App-Android平台 修复 bindingx 执行 evaluateColor 可能出现异常的Bug [详情](https://ask.dcloud.net.cn/question/151759)
  + App-Android平台 修复 uni.reLaunch 打开非 tabbar nvue 页面可能依然显示 tabbar 的Bug [详情](https://ask.dcloud.net.cn/question/143792)
  + App-Android平台 修复 GooglePlay 渠道包无法正常使用高德地图的Bug [详情](https://ask.dcloud.net.cn/question/152668)
  + App-Android平台 修复 nvue 作为首页使用 picker 可能引起应用无响应的Bug [详情](https://ask.dcloud.net.cn/question/151819)
  + App-iOS平台 修复 nvue tabbar 页面 uni.reLaunch 不触发 onUnload 生命周期的Bug [详情](https://ask.dcloud.net.cn/question/152738)
  + Web平台 修复 调用 uni.setClipboardData 会弹起键盘的Bug [详情](https://github.com/dcloudio/uni-app/issues/3569)
  + 小程序平台 优化 小程序组件内部支持使用 kebab-case 事件名 [详情](https://github.com/dcloudio/uni-app/issues/1802)
  + 微信小程序平台 修复 wxs 内调用 triggerEvent 无法携带事件参数的Bug [详情](https://github.com/dcloudio/uni-app/issues/3829)
  + 快手小程序平台 修复 授权手机号的无回调信息的Bug [详情](https://ask.dcloud.net.cn/question/143078)
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 更新 UniPush使用的个推SDK为 3.2.12.0 版，个推核心组件SDK为 3.1.10.0 版，OPPO厂商推送SDK为 3.1.0 版，华为厂商推送SDK为 6.5.0.300 版； 一键登录使用的个验SDK为 3.0.6.0 版；支付宝SDK为 15.8.11 版；新浪微博SDK为 12.5.0 版；友盟统计SDK为 9.5.2 版；解决提交应用市场可能隐私检测被拒的问题 [详情](https://ask.dcloud.net.cn/question/143573)
  + Android平台 修复 getVideoInfo 获取纵向视频文件的宽高值相反的Bug [详情](https://ask.dcloud.net.cn/question/151205)
  + Android平台 修复 previewImage 预览图片时可能出现偏移的Bug [详情](https://ask.dcloud.net.cn/question/151966)
  + iOS平台 修复 uploader 上传文件获取 uploadedSize 值不准确的Bug
* 【uni小程序SDK】
  + iOS平台 修复 uni.setStorage 存储数据可能出错的Bug

## 3.6.0.20220901-alpha
* 【重要】新增 uts语法支持。使用ts开发原生 [详情](https://uniapp.dcloud.io/tutorial/syntax-uts.html)
* 新增 查找引用功能。支持对js、ts变量方法点右键查找
* 优化 Windows 内置浏览器 升级Cef版本到90.6.7
* 新增 HBuilderX设置 插件配置 增加配置项 启用JavaScript校验、启用TypeScript校验
* 新增 语言服务 vue、js内变量语法实时校验（js校验，需要在【设置 - 插件配置】中开启）
* 新增 语言服务 vue3 `style module`支持代码提示
* 新增 语言服务 vue2&3 `插槽`支持代码提示
* 新增 语言服务 vue2&3 script 区域支持自动导包
* 修复 语言服务 vuedoc 在 script setup 内不生效的bug
* 修复 语言服务 vue3 在 script setup 内 import 的自定义组件，在 template 区域无法提示的Bug
* 修复 语言服务 修改函数调用的名称时，会重复生成`()`的Bug
* 修复 语言服务 特殊String 不支持 `if(idstr === '|')` 写法的Bug
* 修复 语言服务 vue template 内变量悬浮不生效的Bug
* 修复 语言服务 uniCloud.importObject()，云对象修改后，代码提示、悬浮不能实时生效的Bug
* 优化 语言服务 uniCloud.importObject()，调用云对象上的方法时参数及返回值的代码提示
* 修复 语言服务 遵循 vetur 规范的 framework包 安装卸载的时候不能实时生效的Bug
* 修复 语言服务 html script 中引用其他文件的变量和函数悬浮不生效的Bug
* 修复 语言服务 html script 中引用其他文件的函数时解析返回值和参数类型不正确的Bug
* 修复 语言服务 底部状态栏框架语法库，移除时无法生效的Bug
* 修复 语言服务 vue cli项目，vue script 区域无法识别项目下 tsconfig.json 的Bug
* 修复 语言服务 修改写好的标签名称时，选择代码提示项后多补内容的Bug
* 优化 语言服务 设置px转rem后，转换提示放到代码提示的第一项
* 新增 标签卡 右键菜单 增加菜单 向左移动标签卡、向右移动标签卡
* 修复 Windows HBuilderX未启动的情况下，导入插件市场插件，首次导入UI视图显示空白的Bug
* 修复 多文件字符搜索 某些情况下，跳转位置错误的Bug
* 修复 转到定义到另一个文件后，后退时，光标跳转到该文件开始，而不是转到定义前的位置的Bug
* 新增 HBuilderX英文 发行 H5发行及小程序发行窗口 窗口UI文本国际化
* 新增 新建项目 HBuilderX插件 增加国际化示例模板
* 修复 uni-app manifest.json 应用名称国际化后，打包界面，应用名称显示%%的Bug
* 调整 uni-app manifest.json 左侧“H5配置”改名为“Web配置”
* 【uni-app插件】
  + 【重要】新增 uts Android版插件 [详情](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html)
  + App-iOS平台 修复 uni.openLocation 底部安全区适配问题 [详情](https://ask.dcloud.net.cn/question/150074)
  + App-iOS平台 修复 uni.chooseLocation 可能引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/152367)
  + Web平台 新增 支持配置和使用高德地图 [详情](https://uniapp.dcloud.io/collocation/manifest?id=h5sdkconfigmaps)
  + 支付宝小程序平台 修复 配置全局小程序组件后编译报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3619)
  + 支付宝小程序平台 修复 启用小程序基础库2.0配置后访问 $slots 报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3529)
  + 字节小程序平台 新增 vue2 项目支持 onUploadDouyinVideo 生命周期 [详情](https://ask.dcloud.net.cn/question/151113)
* 【uniCloud插件】
  + 调整 本地调试插件 云对象运行参数配置文件改为 ${objectName}.param.js [详情](https://uniapp.dcloud.net.cn/uniCloud/rundebug.html#run-obj-param)
  + 修复 本地调试插件 HBuilderX 3.5.5 版本引出的使用 push 扩展库导致其他云函数不能正常运行的Bug
  + 修复 本地调试插件 HBuilderX 3.5.5 版本引出的连接本地云函数时偶发 `SIGN_PARAM_INVALID` 错误
* 【App插件(含5+App和uni-app的App端)】
  + 【重要】Android平台 新增 云端打包支持配置原生应用清单文件 AndroidManifest.xml 和应用资源目录 res、assets [详情](https://uniapp.dcloud.net.cn/tutorial/app-nativeresource-android)
  + Android平台 更新 uni-AD 快手广告SDK Android为 3.3.29 版；快手内容联盟SDK Android为 3.3.31 版
  + Android平台 修复 uni-AD Sigmob激励视频广告点击跳过按钮后关闭触发 onClose 事件返回的 isEnded 属性值可能不准确的Bug
  + Android平台 修复 腾讯云安全检测可能误报`含数字天堂(dcloud)广告插件,可读取设备信息,可能泄露您的个人隐私`的Bug [详情](https://ask.dcloud.net.cn/question/150624)
  + Android平台 修复 安全检测可能报快手广告 SDK 频繁获取用户信息的Bug
  + iOS平台 修复 3.5.0版本引出的 快手开屏广告点击打开落地页返回后无法进入应用首页的Bug [详情](https://ask.dcloud.net.cn/question/152441)
  + iOS平台 修复 未使用Push模块上传 AppStore 报`ITMS-90078: Missing Push Notification Entitlement`警告的Bug

## 3.5.5.20220825-alpha
* 修复 3.5.4引出的 Windows HBuilderX Cli命令失效的Bug
* 新增 App真机运行 设备选择窗口 增加选择基座功能
* 修复 App真机运行 Windows 当项目路径存在中文，运行到 iOS设备，App页面显示异常的Bug
* 修复 App真机运行 某些情况下，安装自定义基座失败的Bug
* 修复 uni-app manifest.json uniPush字段 某些情况下变成 null 的Bug
* 【uni-app插件】
  + 修复 项目路径包含括号时编译异常的Bug [详情](https://ask.dcloud.net.cn/question/150173)
  + App平台 修复 vue 页面 cover-view 组件 flex 布局无效的Bug [详情](https://ask.dcloud.net.cn/question/151697)
  + App平台 修复 vue3 项目 uni.getSystemInfo 获取 windowHeight 值不准确的Bug [详情](https://ask.dcloud.net.cn/question/150862)
  + App平台 修复 vue3 项目 vue 页面 map 组件更新中心坐标后显示错误的Bug [详情](https://ask.dcloud.net.cn/question/151438)
  + App-Android平台 修复 uni.saveImageToPhotosAlbum 保存网络图片可能覆盖上次保存的图片的Bug [详情](https://ask.dcloud.net.cn/question/125357)
  + App-Android平台 修复 picker 组件获取焦点异常的Bug [详情](https://ask.dcloud.net.cn/question/150454)
  + App-Android平台 修复 nvue 页面 map 组件 customCallout 设置图片可能引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/150166)
  + App-iOS平台 修复 uni.getSystemSetting 获取的 bluetoothEnabled、locationEnabled 值不准确的Bug
  + App-iOS平台 修复 nvue 页面 map 组件 marker 调用 moveAlong 方法没有中断前一次动画的Bug [详情](https://ask.dcloud.net.cn/question/151411)
  + App-iOS平台 修复 3.5.2 引出的 nvue 页面 ad-content-page 组件在某些场景可能引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/151778)
  + Web平台 修复 vue3 项目 css 环境变量 --window-top 计算错误的Bug [详情](https://ask.dcloud.net.cn/question/150842)
  + Web平台 修复 vue3 项目发行模式 showLoading 图标大小显示错误的Bug [详情](https://ask.dcloud.net.cn/question/149819)
  + Web平台 修复 custom-tab-bar 组件使用 uni.setTabBarItem 设置 visible 无效的Bug [详情](https://ask.dcloud.net.cn/question/132947)
  + 小程序平台 修复 v-for 内使用复杂表达式后 v-model 失效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3173)
  + 支付宝小程序、百度小程序、快手小程序、字节小程序平台 优化 支持自动拷贝 ext.json 文件
  + 支付宝小程序平台 优化 uni.saveImageToPhotosAlbum 接口不再使用旧版 saveImage 接口
  + 字节小程序平台 修复 vue2 项目 反复快速创建销毁页面时组件无法渲染的Bug
* 【uniCloud插件】
  + 优化 阿里云 数据库超时时间由3秒调整为5秒
  + 新增 阿里云 通过代理解决微信服务器需要固定IP的问题 [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#http-proxy-client)
  + 新增 提供了一批新API，更优雅的处理同实例多并发请求
    - 新增 uniCloud.getRequestList 用于获取当前云函数实例内正在处理的请求的 requestId 列表 [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#get-request-list)
    - 云函数 新增 context.requestId 用于获取当前请求id [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#context)
    - 云对象 新增 this.getUniCloudRequestId() 用于获取当前请求id [详情](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#get-request-id)
  + 新增 云函数 uniCloud.getCloudInfos 获取云端信息。同时兼容有无并发请求的情况 [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#get-cloud-infos)
  + 新增 云函数 uniCloud.getClientInfos 获取客户端信息。同时兼容有无并发请求的情况 [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#get-client-infos)
  + 修复 客户端sdk 未关联 uniCloud 服务空间时使用 uniCloud 对象导致报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3758)
  + 修复 JQL 一个表内多个包含 parentKey 字段时树查询报错的Bug [详情](https://ask.dcloud.net.cn/question/151834)
  + 修复 本地调试插件 部分情况下全局对象复用导致的扩展库提示不正确的Bug [详情](https://ask.dcloud.net.cn/question/150357)
  + 优化 本地调试插件 持续调试会导致内存占用过高并且响应缓慢的Bug
  + 优化 uniIdRouter 支持对首页、直达页面进行拦截并跳转到登录页面
  + 优化 uni-id-co 密码规则调整，废除之前的简单校验，允许配置密码强度 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#password-strength)
  + 调整 uni-id-co 存储用户 openid（`wx_openid.${mp|h5|app|web}`）时同时在`wx_openid.${mp|h5|app|web}_${DCloudAppId}`存储了一份副本，参考：[微信登录](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#login-by-weixin)、[QQ登录](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#login-by-qq)
  + 调整 uni-id-co 依赖 uni-open-bridge-common 存储用户 `session_key`、`access_token` 等凭据 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#save-user-token)
  + 新增 uni-id-co 增加 beforeRegister 钩子用户在注册前向用户记录内添加一些数据 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#before-register)
  + 【重要】新增 uni-id-pages Web端支持微信登录（包括微信公众号内H5登录 和 普通浏览器内手机微信扫码登录）[详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#weixinlogin)
  + 新增 uni-id-pages 支持密码强度（是否必须包含大小写字母、数字和特殊符号以及长度）配置 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#config)
  + 新增 uni-id-pages 登录成功（全局）回调事件：`uni-id-pages-login-success`，支持通过[uni.$on](https://uniapp.dcloud.net.cn/api/window/communication.html#on)监听 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html)
  + 新增 uni-open-bridge 开源库，统一管理微信等三方开放平台的凭据 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-open-bridge.html)
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 更新 QQ 登录、分享SDK版本为 3.5.12 版；百度定位SDK为 9.3.5 版，百度地图SDK为 7.5.3 版
  + Android平台 修复 UniPush 2.0 厂商推送通道不支持 payload 字段为非 json 字符串的Bug
  + Android平台 修复 plus.push.createMessage 创建本地消息 option 参数设置 when 字段无效的Bug
  + Android平台 修复 plus.runtime.install 升级 apk 可能报空指针的Bug
  + iOS平台 更新 uni-AD 百度百青藤广告SDK为 4.891 版
  + iOS平台 修复 3.5.0版本引出的 uni-AD 信息流广告设置宽度可能引起显示异常的Bug [详情](https://ask.dcloud.net.cn/question/150789)
  + iOS平台 修复 3.5.0版本引出的 使用百度定位模块需要勾选IDFA的Bug
  + iOS平台 修复 3.5.3版本引起的 标准真机运行基座中一键登录返回的 token 值不正确的Bug
  + iOS平台 修复 从本地相册中选择慢动作视频显示的时长不准确的Bug [详情](https://ask.dcloud.net.cn/question/150531)
* 【uni小程序SDK】
  + Android平台 优化 默认菜单字体大小为20px

## 3.5.4.20220805-alpha
* 【重要】优化 App真机运行 使用Node运行，不再依赖Java
* 修复 调试视图 变量 Global节点 某些情况下，UI显示错乱的Bug
* 修复 HBuilderX 保存文件 utf-8 格式文件无文件头标识字节 0xEFBBBF的Bug [详情](https://ask.dcloud.net.cn/question/112186)
* 【uni-app插件】
  + App平台 优化 vue2 项目 web-view 组件通过 webviewStyles 设置更多样式 [详情](https://ask.dcloud.net.cn/question/149212)
  + App平台 优化 vue 页面 web-view 组件内页面默认支持绘制到安全区外 [详情](https://ask.dcloud.net.cn/question/149472)
  + App平台 修复 openLocation、chooseLocation 在应用语言改变时没有跟随变化的Bug [详情](https://ask.dcloud.net.cn/question/149216)
  + App-Android平台 新增 uni.scanCode autoZoom 属性，可控制扫码时是否启用自动放大功能 [详情](https://uniapp.dcloud.net.cn/api/system/barcode.html)
  + App-Android平台 修复 nvue map 组件 maker 点聚合坐标重叠无法展现的Bug [详情](https://ask.dcloud.net.cn/question/149665)
  + App-Android平台 修复 nvue map 组件 polyline、polygon 清空数据不生效的Bug
  + App-iOS平台 修复 uni.setTabBarItem 动态更新 icon 可能不生效的Bug [详情](https://ask.dcloud.net.cn/question/149955)
  + App-iOS平台 修复 nvue map 组件使用 Google 地图时，多个页面中使用地图组件可能无法正常加载的Bug [详情](https://ask.dcloud.net.cn/question/150080)
  + Web平台 优化 web-view 组件支持 fullscreen 属性 [详情](https://uniapp.dcloud.net.cn/component/web-view.html)
  + Web平台 修复 vue3 项目 canvas 组件 touch 事件 stop、prevent 修饰符无效的Bug [详情](https://ask.dcloud.net.cn/question/148195)
  + 支付宝小程序平台 修复 vue3 项目 访问 $slots 不生效的Bug [详情](https://ask.dcloud.net.cn/question/150373)
* 【uniCloud插件】
  + 【重要】新增云函数ip防刷功能，避免大量无效请求导致云函数、数据库响应变慢 [详情](https://uniapp.dcloud.net.cn/uniCloud/ip-filter.html)
  + 修复 部分场景下在 main.js 内使用 uniCloud 报错的Bug
  + 修复 uni-admin 在 vue3 项目中使用 uni.showLeftWindow 后组件上 showLeftWindow 值并没有更新的Bug [详情](https://ask.dcloud.net.cn/question/149618)
  + uni统计2 新增 前端数据上报周期配置项 [详情](https://uniapp.dcloud.net.cn/uni-stat-v2.html#report-time)
* 【App插件(含5+App和uni-app的App端)】
  + iOS平台 修复 3.5.0版本引出的 使用百度地图或百度定位时未勾选`使用广告标识（IDFA）`云打包报错的Bug
  + iOS平台 修复 3.5.3版本引出的 开通 uni-AD 开屏广告后台切前台可能导致页面回退不正常的Bug [详情](https://ask.dcloud.net.cn/question/150053)
  + iOS平台 修复 图片选择界面设置 crop 属性选择 iCloud 图片黑屏的Bug [详情](https://ask.dcloud.net.cn/question/149219)

## 3.5.3.20220727-alpha
* 修复 操作系统环境变量 配置NODE_OPTIONS --openssl-legacy-provider后，HBuilderX启动时失去响应的Bug
* 修复 未登录时点击菜单【发行 原生APP-查看云打包状态】闪退的Bug
* 修复 Wap2App项目，提交打包，某些情况下，生成的App样式不正确的Bug
* 修复 uniCloud项目 node_modules文件特别多时，运行项目，Node进程CPU占用率过高的Bug
* 【uni-app插件】
  + App平台 新增 uni.openAppAuthorizeSetting 跳转系统授权管理页 [详情](https://uniapp.dcloud.io/api/system/openappauthorizesetting.html)
  + App-iOS平台 修复 https 请求配置自签名 p12 证书包含中间证书时请求报错的Bug [详情](https://ask.dcloud.net.cn/question/149526)
  + App-iOS平台 修复 nvue box-shadow 样式设置 spread 参数无效的Bug [详情](https://ask.dcloud.net.cn/question/148415)
* 【uniCloud插件】
  + 新增 uni-admin uni统计支持上传 sourceMap，报错可准确回溯源码 [详情](https://uniapp.dcloud.io/uni-stat-v2.html#sourcemap-parse-error)
* 【App插件(含5+App和uni-app的App端)】
  + 更新 uni-AD 腾讯优量汇SDK Android为 4.480.1350 版，iOS为 4.13.80 版；快手广告SDK iOS为 3.3.27 版；今日头条穿山甲SDK iOS为 4.7.0.0 版；穿山甲GroMore广告SDK iOS为 3.5.1.0 版；Sigmob广告联盟SDK iOS为 4.2.1 版
  + Android平台 更新 UniPush 使用的个推SDK为 3.2.11.0 版，个推核心组件SDK为 3.1.9.0 版；谷歌渠道个推SDK为 3.2.10.8 版，个推核心组件SDK为 3.1.9.10 版；解决安全检测可能报个推SDK超频获取信息的问题 [详情](https://ask.dcloud.net.cn/question/149127)
  + Android平台 修复 上架某些应用市场审核检测可能报应用后台运行时存在获取任务列表行为的Bug
  + iOS平台 修复 3.5.0版本引出的 创建本地消息 plus.push.createMessage 不传 option 参数引起应用崩溃的Bug
  + iOS平台 修复 sqlite 在应用 restart 后 executeSql 修改数据报`Attempt to write a readonly database`错误的Bug [详情](https://ask.dcloud.net.cn/question/139765)
  + iOS平台 修复 从本地相册中选择慢动作视频引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/149219)
  + iOS平台 修复 视频播放 video 的 seek 方法传入小于当前播放时间值无效的Bug [详情](https://ask.dcloud.net.cn/question/148781)
  + iOS平台 修复 打开包含视频播放 video 控件的页面会打断其他App后台音乐播放的Bug [详情](https://ask.dcloud.net.cn/question/146719)
* 【uni小程序SDK】
  + iOS平台 修复 未开启后台运行，多次切换小程序和原生界面可能导致小程序返回按钮无效的Bug

## 3.5.2.20220719-alpha
* 新增 语言服务 uni-app i18n国际化 pages.json和Vue页面 支持i18n代码提示、转到定义 [详情](https://uniapp.dcloud.io/tutorial/i18n.html#codeHints)
* 修复 语言服务 await关键字补全 某些情况下，附带多余信息的Bug
* 新增 Markdown 支持跨文件转到#标题或标题的@别名 [详情](https://hx.dcloud.net.cn/Tutorial/Language/markdown?id=goto-definition)
* 优化 插件安装 提示插件安装失败时给出详细原因和解决指南
* 调整 Git插件 pull操作 默认选项改为第四项，即git pull --rebase --autostash
* 修复 3.5.1引出的 弹出快速选择窗口（如Git或语言选择）不响应esc和视图弹出层级错误的Bug
* 修复 App安心打包 某些情况下，提交打包，提示大小超过40M的Bug
* 修复 App manifest.json 一键生成iOS通用链接功能，不能自动生成`apple-app-site-association`文件的Bug [详情](https://ask.dcloud.net.cn/question/149006)
* 新增 海外开发者可使用`HBuilderX国际区账号`进行云端打包 [详情](https://uniapp.dcloud.io/tutorial/internationalization.html)
* 【uni-app插件】
  + App平台 新增 uni.getSystemSetting 获取手机系统的定位、蓝牙、wifi开关等设置 [详情](https://uniapp.dcloud.io/api/system/getsystemsetting)
  + App平台 新增 uni.getAppAuthorizeSetting 获取应用权限状态，是否被授予定位、相册等权限 [详情](https://uniapp.dcloud.io/api/system/getappauthorizesetting)
  + App平台 新增 uni.createPushMessage 创建本地通知栏消息 [详情](https://uniapp.dcloud.io/api/plugins/push.html#createpushmessage)
  + App平台 修复 vue3 项目 首次启动调用 uni.getPushClientId 获取不到cid的Bug
  + App平台 修复 vue2 项目 nvue 页面访问 process.env 报错的Bug [详情](https://ask.dcloud.net.cn/question/147948)
  + App、Web平台 修复 vue3 项目 uni.openLocation 未配置 latitude longitude 时不触发 fail 回调的Bug
  + App-Android平台 修复 nvue map 组件放大地图时标记点气泡 callout 不显示的Bug [详情](https://ask.dcloud.net.cn/question/148741)
  + App-iOS平台 修复 nvue image 组件 src 属性更新使用 gif 格式图片时无法切换的Bug [详情](https://ask.dcloud.net.cn/question/148807)
  + App-iOS平台 修复 nvue 组件动态修改 border-radius 样式可能不生效的Bug [详情](https://ask.dcloud.net.cn/question/144709)
  + 百度小程序平台 修复 vue3 项目 uni.login 失效的Bug [详情](https://ask.dcloud.net.cn/question/117304)
* 【uniCloud插件】
  + 【重要】新增 JQL Cache Redis。将 MongoDB 查询结果缓存到 Redis [详情](https://uniapp.dcloud.net.cn/uniCloud/jql-cache-redis.html)
  + 新增 云对象支持URL化 [详情](https://uniapp.dcloud.net.cn/uniCloud/http.html#cloudobject)
  + 新增 云对象支持定时触发 [详情](https://uniapp.dcloud.net.cn/uniCloud/trigger.html#cloudobject)
  + 新增 uniCloud web控制台支持对服务空间进行成员管理 [详情](https://uniapp.dcloud.io/uniCloud/concepts/space.html#collaboration)
  + 修复 JQL操作成功时新增返回`errCode: 0`，兼容uniCloud响应体规范
  + 调整 uni-id-common 仍将token存储在用户表的token字段内，与旧版本uni-id保持一致
  + 修复 uni-id-common 部分情况下报read property 'reduce' of undefined的Bug
  + 优化 uni-admin 应用管理模块可管理App下载地址、小程序二维码等更多应用信息 [详情](https://uniapp.dcloud.io/uniCloud/admin.html#app-manager)
  + 调整 uni-admin 内置 统一发布页（uni-portal）插件 [详情](https://uniapp.dcloud.io/uniCloud/admin.html#uni-portal)
  + 调整 uni-admin 内置 App升级中心（uni-upgrade-center）插件，并支持多应用商店更新 [详情](https://uniapp.dcloud.io/uniCloud/admin.html#uni-upgrade-center)
  + 新增 uni-id-pages 允许覆盖uni-id-co内置校验规则 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#custom-validator)
  + 修复 uni-id-pages uni-id-co的logout接口时没有删除token的Bug
  + 修复 uni-id-pages app端 clientInfo.appVersionCode 为数字导致 uni-id-co 校验无法通过的Bug
  + 修复 uni-id-pages 微信小程序调用uni-id-co接口报错的Bug [详情](https://ask.dcloud.net.cn/question/148877)
* 【App插件(含5+App和uni-app的App端)】
  + 新增 uni-AD 支持穿山甲GroMore广告 包括开屏、信息流、插屏、全屏视频、激励视频广告
  + 更新 uni-AD 腾讯优量汇SDK Android为 4.472.1342 版；快手广告SDK Android为 3.3.27 版，iOS为 3.3.26 版；快手内容联盟SDK Android为 3.3.30 版；百度百青藤广告SDK Android为 9.223 版，iOS为 4.883 版；Sigmob广告联盟SDK Android为 4.4.0 版；华为广告SDK Android为 13.4.54.300 版
  + iOS平台 修复 3.5.0版本引出的 plus.runtime.restart 重启应用后页面返回按钮失效的Bug
  + iOS平台 修复 3.5.0版本引出的 uni-AD 开通基础广告首次安装可能卡在启动页面的Bug [详情](https://ask.dcloud.net.cn/question/149192)
  + iOS平台 修复 plus.runtime.openWeb 在 iOS15.4 及以上设备打开页面导航栏显示不正常的Bug [详情](https://ask.dcloud.net.cn/question/148585)
  + iOS平台 修复 标题栏 titleNView 更新按钮样式导致布局错位的Bug [详情](https://ask.dcloud.net.cn/question/148542)
  + iOS平台 修复 plus.navigator.getOrientation 在设备横屏状态时返回值不正确的Bug [详情](https://ask.dcloud.net.cn/question/148843)
* 【Uni小程序SDK】
  + iOS平台 修复 偶现内存泄漏可能引起应用崩溃的Bug
  + iOS平台 修复 直达二级页面后再打开此页面，关闭时会直接返回首页的Bug

## 3.5.1.20220707-alpha
* 新增 HBuilderX uniCloud前端网页托管 支持腾讯云
  + 入口1：选中web项目，点击菜单发行-上传网站到服务器
  + 入口2：uni-app发布为H5时，勾选 直接部署到前端网页托管
  + 入口3: HBuilderX CLI 部署和管理前端网页托管 [详情](https://hx.dcloud.net.cn/cli/uniCloud-hosting)
* 新增 HBuilderX 状态栏 右下角补充升级图标及新版本红点提示
* 修复 单项目窗体 编辑器 选择语言关联窗口位置偏移的Bug
* 修复 代码块设置 自定义其它语言代码块 窗口列表出现两个JSON选项的Bug
* 修复 自定义代码块 注释中$DATE_TIME显示日期错误的Bug
* 修复 语言服务 CSS pointer-events缺少auto属性的Bug
* 修复 语言服务 Vue {{}}view后按tab，编辑器右下角弹窗提示Failed to expand abbreviation的Bug
* 修复 语言服务 uni-app项目，import x from ‘@/‘，`@/`开头的路径，某些情况下，转到定义失败的Bug
* 修复 打开内置终端后，插件API hx.window.showQuickPick() 窗口无法滚动的Bug
* 新增 uni-app 新建页面 增加 uni-id-pages 模板 [详情](https://ext.dcloud.net.cn/plugin?name=uni-id-pages)
* 【uni-app插件】
  + 修复 vue3 项目 编译器清空输出目录可能报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3650)
  + App、Web平台 优化 movable-view 组件触摸过程中支持设置 disabled 属性 [详情](https://github.com/dcloudio/uni-app/issues/2384)
  + App平台 修复 map 组件在部分设备显示黑色边框的Bug [详情](https://ask.dcloud.net.cn/question/145449)
  + App平台 修复 vue3 项目 input 绑定动态 type 报错的Bug
  + App平台 修复 vue3 项目 nvue 页面组件插槽样式可能不正确的Bug [详情](https://github.com/dcloudio/uni-app/issues/3632)
  + App平台 修复 vue3 项目 vue 页面在 iOS 平台内存不足导致白屏未自动恢复的Bug [详情](https://ask.dcloud.net.cn/article/35913)
  + App平台 修复 vue3 项目 nvue 页面 webview 组件 onPostMessage 事件无效的Bug [详情](https://ask.dcloud.net.cn/question/144731)
  + App-Android平台 修复 nvue 页面为首页时在部分特定手机启动界面关闭过慢的Bug
  + App-Android平台 修复 nvue image 组件在部分设备可能报空指针错误的Bug [详情](https://ask.dcloud.net.cn/question/147965)
  + App-iOS平台 优化 IAP 支付逻辑 补充手动关闭订单策略，解决自动关单但后续报错可能造成丢单的Bug [详情](https://uniapp.dcloud.net.cn/api/plugins/payment.html#iap)
  + App-iOS平台 修复 uni.getSystemInfo 获取某些设备型号不正确的Bug [详情](https://ask.dcloud.net.cn/question/148344)
  + App-iOS平台 修复 动态设置 tabBar 隐藏再显示后高斯模糊效果失效的Bug [详情](https://ask.dcloud.net.cn/question/146478)
  + App-iOS平台 修复 nvue bindingx 在滚动视图中使用 transform.translateY 结果有偏差的Bug [详情](https://ask.dcloud.net.cn/question/144209)
  + App-iOS平台 修复 nvue input 组件嵌套在 list 中时，页面上下滑动 v-model 绑定的值会置空的Bug [详情](https://ask.dcloud.net.cn/question/146246)
  + App-iOS平台 修复 nvue textarea 组件设置 auto-height 为 true 时初始高度不正确的Bug [详情](https://ask.dcloud.net.cn/question/146688)
  + Web平台 补齐 vue2 项目支持 uni.getLaunchOptionsSync [详情](https://uniapp.dcloud.net.cn/api/getLaunchOptionsSync.html)
  + Web平台 补齐 vue2 项目支持 uni.getEnterOptionsSync [详情](https://uniapp.dcloud.net.cn/api/getEnterOptionsSync.html)
  + Web平台 优化 hover-class 支持鼠标事件
  + Web平台 优化 map 组件 markertap 事件支持返回坐标信息
  + Web平台 修复 map 组件 tap 事件重复触发的Bug
  + 小程序平台 优化 vue2 项目 slot name 支持动态赋值 [详情](https://ask.dcloud.net.cn/question/82506)
  + 小程序平台 修复 vue3 项目部分情况下，编译后组件 js 文件名不正确的Bug [详情](https://github.com/dcloudio/uni-app/issues/3629)
  + 小程序平台 修复 vue3 项目部分情况下，数据更新后，页面未渲染的Bug [详情](https://github.com/dcloudio/uni-app/issues/3648)
  + 小程序平台 修复 vue2 项目命名插槽使用 v-if 编译报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/2635)
  + 微信小程序、支付宝小程序平台 新增 vue3 项目 manifest.json 支持 mergeVirtualHostAttributes 配置，用于合并虚拟节点外部样式 [详情](https://uniapp.dcloud.io/collocation/manifest.html#mp-weixin)
  + 百度小程序、字节小程序平台 修复 vue3 项目 部分情况下，组件 ref 获取不到的Bug [详情](https://github.com/dcloudio/uni-app/issues/3615)
  + 百度小程序、字节小程序平台 修复 vue3 项目 组件事件名包含`-`或`:`时，无法触发的Bug [详情](https://github.com/dcloudio/uni-app/issues/3616)
  + 微信小程序平台 修复 vue3 项目 input 组件动态 type 在 iOS 平台不生效的Bug [详情](https://ask.dcloud.net.cn/question/147787)
  + 微信小程序平台 修复 vue3 项目 微信开发者工具中配置编译模式丢失的Bug [详情](https://github.com/dcloudio/uni-app/issues/3655)
  + 微信小程序平台 修复 vue3 项目 project.config.json 更新可能导致开发者工具报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3524)
  + 百度小程序平台 修复 vue3 项目 事件触发可能混乱的Bug[详情](https://github.com/dcloudio/uni-app/issues/3647)
  + 字节小程序平台 修复 vue3 项目 部分情况下，组件未更新的Bug [详情](https://github.com/dcloudio/uni-app/issues/3625)
* 【uniCloud插件】
  + 【重要】新增 uni-push2.0 全端支持（App、小程序、web）的云端一体的统一推送服务 [详情](https://uniapp.dcloud.io/unipush-v2.html)
  + 新增 腾讯云平台 数据万象，对云存储文件进行图片缩放、增加水印等计算功能 [详情](https://uniapp.dcloud.net.cn/uniCloud/storage.html#%E6%95%B0%E6%8D%AE%E5%A4%84%E7%90%86)
  + 新增 keepRunningAfterReturn 配置云函数是否能在 return 后继续运行，仅腾讯云 nodejs12 生效 [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#keep-running)
  + 新增 Redis扩展库 增加 quit 接口用于断开 redis 连接 [详情](https://uniapp.dcloud.net.cn/uniCloud/redis.html#quit)
  + 新增 JQL数据库管理 支持使用更新操作符 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql.html#update-command)
  + 修复 uniIdRouter 在 loginPage 为 tabbar 页面时无法自动跳转的Bug
  + 调整 云函数 context 内增加 `uniIdToken`、`FUNCTION_TYPE` [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-callfunction.html#context)
  + 调整 云对象 cloudInfo 内增加 functionName、functionType [详情](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#get-cloud-info)
  + 调整 云对象 clientInfo 内增加 source [详情](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#get-client-info)
  + 修复 本地调试插件 使用运行菜单运行云函数时可能出现日志顺序错误的Bug
  + 修复 本地调试插件 项目AppId由无权使用调整为有权使用时（重新获取AppId或获得所有者授权）重启项目不生效的Bug
  + 调整 本地调试插件 云函数本地运行时配置的运行参数clientInfo内字段调整 [详情](https://uniapp.dcloud.net.cn/uniCloud/rundebug.html#mock-client-info)
  + 新增 HBuilderX opendb schema文件 右键菜单增加【opendb检查更新】，支持从云端更新 opendb schema文件，并生成 JQL 升级迁移文件用于数据迁移
  + 修复 HBuilderX 打开云对象子目录下的文件时按 Ctrl+r 运行菜单无运行云对象选项的Bug
  + 【重要】调整 uni统计2 版本记录复用 uni升级中心 的 opendb-app-versions表，废弃 uni-stat-app-versions表 [详情](https://uniapp.dcloud.net.cn/uni-stat-v2.html#upgrade)
  + uni统计2 新增 启动时上报设备各种参数入库 opendb-device 表（目前没有可视化报表，开通 uni-push2.0 与 uni统计2.0 自动上报 push_clientid 到 opendb-device表）
  + uni统计2 新增 admin端 app崩溃统计页面，补充崩溃率统计
  + uni统计2 修复 admin端 js报错统计页面，错误率计算不准确的Bug
  + uni统计2 修复 admin端 切换版本或者修改时间等操作后，趋势图状态显示不正确的Bug
  + uni统计2 修复 admin端 部分页面首次进入时界面闪烁的问题
* 【App插件(含5+App和uni-app的App端)】
  + 优化 uni-AD 激励视频和信息流广告支持并发请求
  + Android平台 新增 Google Pay 支持配置支付网关信息 buildTokenizationSpecification [详情](https://uniapp.dcloud.io/tutorial/app-payment-google.html#%E4%BD%BF%E7%94%A8google%E6%94%AF%E4%BB%98)
  + Android平台 更新 腾讯X5内核为 4.3.0.299 版
  + Android平台 新增 Facebook 登录 SDK 为 12.0.0 版，解决登录受限的问题 [详情](https://ask.dcloud.net.cn/question/147788)
  + Android平台 修复 3.5.0 版本引出的 uni-AD 特定情况可能只展示同一广告源广告的Bug
  + Android平台 修复 uploader 上传文件请求返回错误响应码时，无法获取服务器返回数据的Bug
  + Android平台 修复 setBadgeNumber 设置角标在新荣耀设备不生效的Bug [详情](https://ask.dcloud.net.cn/question/140910)
  + iOS平台 新增 IAP支付 手动关闭订单、获取未关闭订单列表等功能，以解决自动关闭订单在某些情况引发的订单丢失的Bug [详情](https://uniapp.dcloud.io/tutorial/app-payment-aip.html)
  + iOS平台 修复 3.5.0 版本引出的 uni-AD 穿山甲开屏广告偶现 bottomView 没有关闭的Bug
  + iOS平台 修复 首次启动 App 获取安全区域高度可能不正确的Bug [详情](https://ask.dcloud.net.cn/question/148277)
  + iOS平台 修复 设备型号名称 model、deviceModel 返回值不规范的Bug
* 【Uni小程序SDK】
  + Android平台 修复 getAppRuningForAppid 在部分场景可能报空指针错误的Bug
  + iOS平台 修复 小程序未开启后台运行，前台运行时调用 open 方法直达页面无效的Bug

## 3.5.0.20220623-alpha
* 新增 uni-app 运行到 Web 时支持 debug 调试 [详情](https://hx.dcloud.net.cn/Tutorial/debug/h5-debug)
* 新增 TypeScript 实时语法校验 [详情](https://hx.dcloud.net.cn/Tutorial/UserGuide/tsSyntaxCheck)
* 新增 语言服务 支持tailwindcss提示，需要安装tailwindcss插件 [详情](https://ext.dcloud.net.cn/plugin?id=8560)
* 新增 MarkDown 代码区块的语言着色高亮，支持提示下载对应语言着色扩展插件
* 修复 语言服务 React 某些情况下，<App />回车后补充了`()`的Bug
* 修复 语言服务 React jsx文件 没有代码提示的Bug
* 修复 首次打开文档并编辑，第一次撤销后光标位置不对的Bug
* 修复 json文件 查找索引符号导致崩溃的Bug
* 新增 uni-app pages_init机制，导入 uni-app 插件到项目下时，可合并新页面路由到项目的 pages.json 中 [详情](https://uniapp.dcloud.io/plugin/uni_modules.html#pages-init)
* 新增 uni-app manifest.json 可视化界面基础配置 增加国际化语言配置 [详情](https://uniapp.dcloud.net.cn/tutorial/i18n.html#manifest)
* 调整 uni-app manifest.json 可视化界面去除微信登录的 AppSecret 输入框，仍可在源码视图填写，但不推荐在前端暴露 AppSecret
* 调整 uni-app manifest.json App常用其它配置，生成 iOS符号表文件，将配置项调整到原生App-云打包窗口
* 【uni-app插件】
  + 新增 App-Android平台 manifest.json 支持最低要求 webview 配置，系统 webview 低于指定版本时，弹出提示或者下载 x5 内核后继续启动 [详情](https://uniapp.dcloud.net.cn/collocation/manifest.html#appwebview)
  + 新增 vue2项目 支持使用 `@/pages.json` 引用条件编译后的 `pages.json` 文件
  + 修复 3.4.17 版本引发的 vue3 项目 运行在小程序平台 `<script setup>`中使用 const 定义 reactive 对象访问出错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3606)
  + App、Web平台 修复 3.4.10 版本引出的 vue2项目 image 组件 load 事件图像大小信息不准确的Bug [详情](https://ask.dcloud.net.cn/question/147174)
  + App平台 优化 slot name 支持动态赋值 [详情](https://ask.dcloud.net.cn/question/95109)
  + App-Android平台 修复 tabbar 启用高斯模糊后获取 windowBottom 错误的Bug [详情](https://ask.dcloud.net.cn/question/146583)
  + App-iOS平台 修复 uni.request 访问特定接口可能数据解析出现乱码的Bug [详情](https://ask.dcloud.net.cn/question/145530)
  + 微信小程序、支付宝小程序 新增 vue2 项目 manifest.json 支持 mergeVirtualHostAttributes 配置，用于合并虚拟节点外部样式 [详情](https://uniapp.dcloud.io/collocation/manifest.html#mp-weixin)
  + 百度小程序平台 修复 vue3 项目 组件嵌套使用时响应式可能失效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3612)
* 【uniCloud插件】
  + 【重要】uni-id重构。`uni-id公共模块` + `uni-id-cf云函数` 的组合不再更新，取而代之的是 `uni-id-common公共模块` + `uni-id-pages云端一体模板`
    - 新增 uni-id-common公共模块。更小巧的公共模块，负责 uni-id 的 token 管理和权限校验 [详情](https://uniapp.dcloud.io/uniCloud/uni-id-common.html)
    - 新增 uni-id-pages云端一体页面模板。包括一组前端页面 + uni-id-co云对象。包括用户注册、登录、忘记密码、个人中心等功能 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html)
  + 新增 uniIdRouter路由管理。在 pages.json 里直接定义哪些页面需要登录后才能访问 [详情](https://uniapp.dcloud.io/uniCloud/uni-id-summary.html#uni-id-router)
  + 新增 uniCloud.onNeedLogin/offNeedLogin 用于监听/移除监听需要登录事件，需搭配 `uniIdRouter` 使用 [详情](https://uniapp.dcloud.io/uniCloud/client-sdk.html#on-need-login)
  + 新增 uniCloud.onRefreshToken/offRefreshToken 用于监听/移除监听 token 更新事件 [详情](https://uniapp.dcloud.io/uniCloud/client-sdk.html#on-refresh-token)
  + 调整 HBuilderX 中创建 uniCloud 项目时默认导入 `uni-id-common公共模块`，不再导入老版 `uni-id公共模块`
  + 调整 clientDB 优先依赖 `uni-id-common`，在没有 `uni-id-common` 时依赖老版 `uni-id公共模块`
  + 修复 本地调试插件 HBuilderX 3.4.12引出的运行项目时部分场景下访问非关联服务空间云函数报错的Bug
  + 修复 本地调试插件 部分app平台、web平台切换云端云函数/本地云函数无效的Bug [详情](https://ask.dcloud.net.cn/question/147633)
  + 修复 clientDB action 的 after 内抛出错误不能被另一个 action 的 after 接收到的Bug [详情](https://ask.dcloud.net.cn/question/147099)
  + 修复 项目内无 uni-id 时运行 jql 文件报错的Bug
  + uniCloud控制台 新增 Redis 数据可视化管理
* 【App插件(含5+App和uni-app的App端)】
  + 【重要】uni-AD 新增 激励视频广告支持实时竞价 [详情](https://uniapp.dcloud.io/uni-ad.html#bidding)
  + Android平台 更新 云端打包环境 Gradle 为 7.3.3，Android Gradle plugin 为 4.2.0，compileSdkVersion 为 31
  + Android平台 新增 云端打包支持设置 dataBinding、viewBinding [文档](https://uniapp.dcloud.io/collocation/manifest.html#buildfeatures)
  + Android平台 修复 startBluetoothDevicesDiscovery 搜索附近蓝牙设备在 Android12 设备可能引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/146849)
  + Android平台 修复 UniPush 存在监听`ACTION_BOOT_COMPLETED`广播行为，可能违反应用市场上架合规检测问题 [详情](https://ask.dcloud.net.cn/question/147319)
  + Android平台 修复 UniPush 调用 plus.runtime.restart 后无法创建本地通知消息的Bug [详情](https://ask.dcloud.net.cn/question/146470)
  + Android平台 修复 从本地相册选择大图片预览时可能引起应用崩溃的Bug
  + iOS平台 更新 uni-AD 今日头条穿山甲SDK为 4.5.1.6 版
  + iOS平台 更新 百度定位SDK为 2.0.0 版，百度地图SDK为 6.5.0 版
  + iOS平台 修复 5+App项目获取 5G 网络类型错误的Bug
* 【Uni小程序SDK】
  + Android平台 修复 启动小程序直达页面参数与文档规范不一致的Bug

## 3.4.17.20220614-alpha
* 修复 Windows 终端开启时，工具栏搜索分类，鼠标移动上去后，悬停列表自动消失的Bug [详情](https://ask.dcloud.net.cn/question/146695)
* 修复 App 原生App-云打包 某些情况下，点击打包没有提交到云端打包的bug
* 修复 uniCloud 前端网页托管 上传网站到服务器，非项目成员进行上传操作，编辑器闪退的Bug
* 【uni-app插件】
  + 修复 vue3 项目 onError 生命周期不生效的Bug
  + App、Web平台 修复 vue3 项目 uni.setTabBarItem 设置 pagePath 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3592)
  + App平台 优化 video 组件支持 show-mute-btn 配置
  + App平台 优化 vue3 项目 rich-text 组件支持服务端渲染
  + App平台 修复 3.4.10 版本引出的 scopeId 污染 slot 导致样式异常的Bug [详情](https://ask.dcloud.net.cn/question/145366)
  + App平台 修复 调试时调用 uni.getSystemInfo 报错的Bug [详情](https://ask.dcloud.net.cn/question/146611)
  + App平台 修复 vue3 项目 Windows 系统上，运行至手机或模拟器时，可能多次同步文件的Bug
  + App平台 修复 vue3 项目 nvue 页面 onPageScroll，onReachBottom 不触发的Bug [详情](https://ask.dcloud.net.cn/question/145873)
  + App平台 修复 vue3 项目 uni.getVideoInfo 成功回调不执行Bug
  + App-Android平台 修复 nvue web-view 组件 user-agent 不正确导致加载H5页面显示异常的Bug [详情](https://ask.dcloud.net.cn/question/146877)
  + App-Android平台 修复 nvue 组件同时设置 box-shadow、elevation 样式在部分特殊场景可能会出现渲染异常的Bug [详情](https://ask.dcloud.net.cn/question/147041)
  + iOS平台 修复 nvue ad-content-page 组件暂停后展示其它视频类广告，关闭广告可能引起组件后台自动播放的Bug
  + Web平台 修复 vue3 项目 pc端 createSelectorQuery 获取 top 错误Bug
  + 小程序平台 修复 vue3 项目 v-for 嵌套使用 slot 时，渲染不正确的Bug [详情](https://github.com/dcloudio/uni-app/issues/3587)
  + 微信小程序平台 修复 3.4.13 版本引出的 manifest.json 文件缺少 mp-weixin 节点编译报错的Bug [详情](https://ask.dcloud.net.cn/question/146580)
* 【uniCloud插件】
  + 修复 本地调试插件 3.4.0版本引出的客户端连接本地云函数时获取客户端 userAgent 为`HBuilderX`的Bug
  + 修复 本地调试插件 云函数内使用`console.timeEnd`输出日志错乱的Bug
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 修复 uni-AD 开屏广告在部分小米手机可能会卡在启动界面的Bug
  + iOS平台 更新 uni-AD 快手广告SDK为 3.3.25 版，快手内容联盟SDK为 3.3.29 版，解决调用系统相册可能引起崩溃的问题

## 3.4.13.20220601-alpha
* 新增 语言服务 JavaScript 支持document.getElementById、document.querySelector中id选择器的dom类型识别
* 新增 语言服务 scss 支持提示`!global` `!default`
* 修复 语言服务 CSS `{}`内，输入`mar`等，max-resolution等媒体查询出现在代码助手第一项的Bug
* 修复 语言服务 JavaScript JQuery代码提示，某些情况下，在`$("")`内输入`#`，回车后，出现两个`#`的Bug
* 修复 语言服务 Vue style节点，输入scoped后，自动补上了`=""`的Bug
* 修复 语言服务 uni-app项目，scss嵌套语法，无法提示uni-app相关标签的Bug
* 修复 语言服务 uni-app项目，import x from ‘@/‘，`@/`开头的路径，某些情况下，转到定义失败的Bug
* 修复 语言服务 uni-app项目，pages.json 条件编译产生语法不对的情况时，导致vue下class没有提示的Bug
* 修复 App 真机运行 某些情况下，查找不到Android设备的Bug
* 修复 App 某些情况下，制作应用wgt包失败的Bug
* 修复 3.4.10引出的 App打包 manifest.json选择云端原生插件，提交云端打包，用户本地配置的插件资源没有上传的Bug
* 【uni-app插件】
  + App、H5平台 新增 uni.getDeviceInfo [详情](https://uniapp.dcloud.io/api/system/getDeviceInfo.html)
  + App、H5平台 新增 uni.getAppBaseInfo [详情](https://uniapp.dcloud.io/api/system/getAppBaseInfo.html)
  + App、H5平台 新增 uni.getWindowInfo [详情](https://uniapp.dcloud.io/api/system/getWindowInfo.html)
  + App、H5平台 新增 uni.getSystemInfo 添加 devicePixelRatio、deviceOrientation、appLanguage 等字段 [详情](https://uniapp.dcloud.io/api/system/info.html)
  + App、H5平台 修复 uni.canIUse 获取某些 api 使用情况，值不正确的Bug [详情](https://uniapp.dcloud.io/api/caniuse.html)
  + App平台 新增 uni.getSystemInfo 添加 romName、romVersion 字段 [详情](https://uniapp.dcloud.io/api/system/info.html)
  + App平台 修复 3.4.10 版本引出的 view 组件使用 wxs/renderjs 报错的Bug
  + App-Android平台 修复 使用谷歌地图时，mapContext 对象调用 moveAlong 移动 marker 动画过程中拖拽地图会产生偏移的Bug
  + App-Android平台 修复 nvue view 组件 hover-class 属性动态改变组件大小时无效的Bug [详情](https://ask.dcloud.net.cn/question/145677)
  + App-iOS平台 修复 nvue 页面滚动视图中设置 position 属性为 sticky 样式显示不正确的Bug [详情](https://ask.dcloud.net.cn/question/144303)
  + H5平台 修复 vue3 项目 当 App.vue 使用 setup 时，发行后页面空白的Bug [详情](https://ask.dcloud.net.cn/question/146011)
  + H5平台 修复 3.4.10 版本引发的 vue3 项目在 left/top/right window 页面使用 match-media 报错的Bug [详情](https://ask.dcloud.net.cn/question/146126)
  + 小程序平台 修复 uni.getLocale 获取值不统一的Bug [详情](https://uniapp.dcloud.io/api/ui/locale.html)
  + 微信小程序平台 修复 vue3 项目 ad-custom 组件无法使用的Bug [详情](https://ask.dcloud.net.cn/question/145883)
* 【uniCloud插件】
  + 新增 uniCloud.onResponse/offResponse 接口用于监听云函数、云对象及clientDB的响应结果 [详情](https://uniapp.dcloud.net.cn/uniCloud/client-sdk.html#on-response)
  + 新增 uniCloud响应体规范 添加 newToken 字段，用于token续期。云对象会自动将token持久化存储 [详情](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#resformat)
  + 修复 uniCloud虚拟目录、以及uni_modules下的云对象目录，右键菜单，没有运行-本地云对象、调试运行-本地云对象的菜单的Bug
  + uniCloud控制台 新增 腾讯云云存储支持上传文件夹
  + uni-admin 新增 uni统计 可通过选择「应用版本」查询数据
  + uni-admin 新增 uni统计 原生 app 崩溃页部分功能
  + uni-admin 修复 uni统计 渠道页 table 表格最后一列空白的 bug
  + uni-admin 修复 uni统计 场景分析页趋势图有数据却显示为 0 的 bug
  + uni-admin 修复 系统设置中权限只能加载 20 条的 bug
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 新增 原生隐私政策提示框支持 hrefLoader 属性，配置提示框中点击 href 链接的打开方式 [详情](https://uniapp.dcloud.io/tutorial/app-privacy-android)
  + Android平台 修复 uni-AD 腾讯优量汇广告联盟部分下载类广告下载成功之后无法安装的Bug
  + iOS平台 更新 一键登录 使用的个验SDK为 2.2.0.0 版，个推核心组件SDK为 1.2.7.0 版
  + iOS平台 修复 音频播放 audio 设置 startTime 可能不生效的Bug [详情](https://ask.dcloud.net.cn/question/146028)
  + iOS平台 修复 视频播放 video 播放 rtmp 协议直播流视频时声音只能通过扬声器播放的Bug [详情](https://ask.dcloud.net.cn/question/129703)
  + iOS平台 修复 视频播放 video 播放 rtmp/rtsp 协议视频时 timeupdate 事件返回当前播放时间 currentTime 始终为 0 的Bug
* 【Uni小程序SDK】
  + Android平台 修复 小程序应用资源更新可能引起页面卡顿的Bug
  + iOS平台 修复 存在自定义 UIWindow 时 toast 可能无法显示的Bug

## 3.4.12.20220523-alpha
* 修复 3.4.10 引出的 项目管理器 项目名称后面没有显示Git分支信息的Bug [详情](https://ask.dcloud.net.cn/question/145569)
* 修复 5+App、wap2App项目 制作应用wgt包失败的Bug
* 【uniCloud插件】
  + 修复 HBuilderX 3.4.10 引起的关联服务空间运行云函数错误的Bug [详情](https://ask.dcloud.net.cn/question/145551)

## 3.4.11.20220520-alpha
* 优化 HBuilderX 启动速度
* 修复 3.4.10引出的 欢迎页面 状态栏选择语言后出现崩溃的Bug
* 修复 3.4.10引出的 php文件 代码没有着色的Bug
* 新增 uniCloud 新建DB Schema 模板列表 支持搜索
* 【uni-app插件】
  + App平台 修复 nvue 页面 switch 组件切换状态无限闪动的Bug [详情](https://ask.dcloud.net.cn/question/145272)
  + App平台 修复 纯 nvue 编译模式 uni_modules 内静态资源未拷贝的Bug
  + App-iOS平台 修复 vue3 项目 nvue 页面 swiper 组件面板指示点无法隐藏的Bug [详情](https://ask.dcloud.net.cn/question/145097)
  + H5平台 新增 vue3 项目 unicloud-db 组件属性 ssr-key [详情](https://uniapp.dcloud.net.cn/uniCloud/unicloud-db.html#ssrkey)
  + H5平台 修复 vue3 项目 unicloud-db 组件 使用 ssr 时 页面存在2个以上组件时数据显示错乱的Bug [详情](https://ask.dcloud.net.cn/question/139537)
  + H5平台 修复 3.4.10 版本引出的 vue2 项目启用摇树优化缺失 view 组件的Bug [详情](https://ask.dcloud.net.cn/question/145286)
  + 小程序平台 修复 vue3 项目 在模板中使用 wxs、sjs 插值表达式不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3527)
  + 支付宝小程序平台 修复 vue3 项目 全局组件不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3525)
  + 支付宝小程序平台 修复 vue3 项目 sjs 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3527)
* 【uniCloud插件】
  + uni-admin 优化 首页增加uni统计的设备概览、注册用户概览
  + uni-admin 优化 登录速度
  + uni-admin 修复 从「首页」跳转「概况」时，url 的 query 丢失的 bug
  + uni-admin 修复 路由改变后面包屑未响应的 bug
* 【App插件(含5+App和uni-app的App端)】
  + 更新 uni-AD 今日头条穿山甲SDK Android为 4.5.1.1 版；腾讯优量汇SDK iOS为 4.13.65 版；快手广告SDK Android为 3.3.24 版，iOS为 3.3.24 版；百度百青藤广告SDK Android为 9.212 版，iOS为 4.87 版；Sigmob广告联盟SDK Android为 3.5.9 版

## 3.4.10.20220517-alpha
* 新增 Node程序 支持运行和调试 [详情](https://hx.dcloud.net.cn/Tutorial/extension/node-development)
* 新增 可自主扩展新语言的语法高亮，可开发或下载语言高亮插件 [详情](https://hx.dcloud.net.cn/Tutorial/Language/language_grammars)
* 调整 部分内置的语言语法高亮迁移到插件市场 [详情](https://hx.dcloud.net.cn/Tutorial/Language/language_grammars?id=list)
* 新增 语言服务 vue-cli项目 支持element-ui、bootstrap-vue等代码提示
* 修复 语言服务 Emmet语言 某些情况下，按下tab，没有反应的Bug
* 修复 语言服务 CSS 在同一行输入CSS代码，回车后，某些情况下，替换位置错误的Bug
* 修复 语言服务 jsdoc代码块替换位置错误的Bug
* 修复 插件安装窗口 已安装插件 某些情况下，版本号显示错误的Bug
* 修复 多文件搜索 某些情况下，右侧栏显示的代码着色错误的Bug
* 调整 App 原生App-云打包 java库改为openjdk
* 优化 App MacOSX 运行到iOS模拟器的窗口增加搜索功能
* 【uni-app插件】
  + 【重要】新增 uni统计2.0版本发布，开源、私有部署、易定制 [详情](https://uniapp.dcloud.net.cn/uni-stat-v2.html)
  + 【重要】uniAD 支持微信小程序平台，降低开通流量主门槛 [详情](https://uniapp.dcloud.net.cn/component/ad-weixin.html)
  + 【重要】App平台 优化 vue2 项目 view 组件实现方式，提高渲染性能。建议相关开发者升级
  + 新增 uni.getSystemInfo 支持获取更多属性 [详情](https://uniapp.dcloud.io/api/system/info.html)
  + 优化 vue3 项目 兼容 pnpm@7.0.0
  + 修复 vue3 项目 部分情况下错误信息不准确的Bug
  + 修复 vue3 项目 vite.config.js 配置 build.minify 为 terser 不生效的Bug [详情](https://ask.dcloud.net.cn/question/144992)
  + App、H5平台 优化 image 组件减少网络请求
  + App、H5平台 修复 canvas transform 渲染时没有使用高清处理的Bug [详情](https://ask.dcloud.net.cn/question/144676)
  + App平台、微信小程序平台 新增 vue3 ad-rewarded-video 激励视频广告组件，更加易用 [详情](https://uniapp.dcloud.net.cn/component/ad-rewarded-video.html)
  + App平台、微信小程序平台 新增 vue3 ad-interstitial 插屏广告组件 [详情](https://uniapp.dcloud.net.cn/component/ad-interstitial.html)
  + App平台 新增 vue3 ad-fullscreen-video 全屏视频广告组件 [详情](https://uniapp.dcloud.net.cn/component/ad-fullscreen-video.html)
  + App平台 修复 vue3 项目使用录音时报错的Bug [详情](https://ask.dcloud.net.cn/question/144821)
  + App平台 修复 vue3 项目 纯 nvue 项目编译报错的Bug
  + App平台 修复 nvue 页面列表删除渲染卡顿的Bug [详情](https://ask.dcloud.net.cn/question/144110)
  + App平台 修复 nvue 页面 transition 包含多个属性时编译报错的Bug [详情](https://ask.dcloud.net.cn/question/89110)
  + App-Android平台 补齐 tabBar 和 navigationBar 支持高斯模糊效果 [详情](https://uniapp.dcloud.io/tutorial/app-blureffect)
  + H5平台 修复 rich-text 组件部分标签没有加上 scopeId 导致样式应用不上的Bug [详情](https://ask.dcloud.net.cn/question/144042)
  + H5平台 修复 vue3 项目使用 picker 组件报错的Bug [详情](https://ask.dcloud.net.cn/question/144073)
  + H5平台 修复 vue3 项目 当页面同时存在 vue、nvue 时，样式不正确的Bug [详情](https://ask.dcloud.net.cn/question/144687)
  + H5平台 修复 vue3 项目 App.vue 使用 setup 不生效的Bug [详情](https://ask.dcloud.net.cn/question/144672)
  + H5平台 修复 vue3 项目 使用 Vue.js devtools 查看页面状态不显示的Bug [详情](https://github.com/dcloudio/uni-app/issues/3492)
  + 小程序平台 修复 vue3 项目 部分情况下代码分割错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/3491)
  + 微信小程序平台 调整 ad 广告组件 [详情](https://uniapp.dcloud.net.cn/component/ad.html#weixin)
* 【uniCloud插件】
  + 新增 本地云函数调用云端redis，方便开发调试 [详情](https://uniapp.dcloud.net.cn/uniCloud/redis.html#lcoal-function)
  + 新增 uni-cloud-jql 扩展库 databaseForJQL 方法支持传递 clientInfo，以便于在云对象中使用 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql-cloud.html#use-in-object)
  + 修复 本地运行插件 HBuilderX 3.4.8 引发的运行云函数时如未绑定服务空间会导致运行进程卡住的Bug
  + 修复 云对象 _before 内抛出错误后 _after 不执行的Bug [详情](https://ask.dcloud.net.cn/question/145046)
  + uni-id 调整 绑定、解绑邮箱手机号接口，只要传递 code 参数就进行验证码校验即使传递的值为undefined
  + uni-id 调整 用户表 `register_env` 内增加 `os_name` 字段用于区分注册时的客户端系统类型
  + uni-id 修复 addUser 接口添加的用户无法使用密码登录的Bug [详情](https://ask.dcloud.net.cn/question/144670)
  + uni-id 修复 config 文件语法错误时报`this.t is not a function`的Bug
  + uni-captcha 新增 集成：创建、刷新、显示验证码的云端一体组件 [详情](https://ext.dcloud.net.cn/plugin?id=4048)
  + uni-starter 新增 短信验证码登陆、绑定手机号码，防刷逻辑；当短信验证码输入错误超过2次，弹出图形验证码进行人机校验。[详情](https://ext.dcloud.net.cn/plugin?id=5057)
  + uni-admin 新增 uni统计数据报表功能 [详情](https://ext.dcloud.net.cn/plugin?id=3268)
* 【Uni小程序SDK】
  + Android平台 修复 多进程模式下微信分享过程中手动返回页面显示异常的Bug
  + Android平台 修复 3.4.7版本引出的 宿主事件回调格式异常的Bug

## 3.4.9.20220508-alpha
* 修复 语言服务 uni-app pages.json easycom节点配置错误时，uview-ui没有代码提示的Bug
* 【uni-app插件】
  + uni统计 修复 3.4.8 版本引发的上报数据不正常的Bug [详情](https://ask.dcloud.net.cn/question/144408)
  + App-iOS平台 修复 nvue textarea 组件默认换行不生效的Bug [详情](https://ask.dcloud.net.cn/question/143784)
  + App-iOS平台 修复 nvue map 组件开启标记点聚合时，调用 removeMarkers 移除所有 marker 引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/143991)
* 【App插件(含5+App和uni-app的App端)】
  + 修复 音频播放 AudioPlayer 暂停后设置播放倍速大于 0 会自动触发播放的Bug [详情](https://ask.dcloud.net.cn/question/143757)
  + Android平台 修复 uni-AD 开屏广告开通腾讯优量汇可能引起应用启动白屏的Bug
  + iOS平台 修复 登录鉴权、分享的 authorize 方法传入认证参数 options 不生效的Bug
* 【uniCloud插件】
  + 【重要】调整 vue2版本客户端App平台对应的`context.PLATFORM`值由 `app-plus` 改为 `app`。此调整对 uni-id 有影响，详情请参考文档：[uni-id preferedAppPlatform](https://uniapp.dcloud.net.cn/uniCloud/uni-id.html#prefered-app-platform)
  + 修复 云对象 自动展示交互界面时未能显示 loading 标题的Bug [详情](https://ask.dcloud.net.cn/question/144526)
  + 调整 客户端将上报所有`getSystemInfoSync`返回的内容供云端使用，参考文档：[云函数内获取客户端信息](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#client-info)，[云对象内获取客户端信息](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#get-client-info)
  + uni-id 新增 getWeixinUserInfo 用于获取app平台微信登录用户的用户信息 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id.html#get-weixin-user-info)
  + uni-id 新增 addUser 用于手动添加用户 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id.html#add-user)
  + uni-id 新增 resetPwdBySms 用于使用短信验证码重置密码 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id.html#reset-pwd-by-sms)
  + uni-id 调整 用户注册时记录用户注册环境到 register_env 字段 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id.html#user-table)
  + uni-id 调整 用户注册时将注册 ip 移至 register_env 内

## 3.4.8.20220428-alpha
* 新增 支持自定义项目级代码块（菜单【工具 代码块设置 自定义项目代码块】）[详情](https://hx.dcloud.net.cn/Tutorial/Language/Snippets?id=projectsnippets)
* 修复 语言服务 vue3, template内，无法提示使用ref函数创建的对象数据的Bug
* 修复 语言服务 html a标签 target属性，没有自动拉出代码候选项的Bug [详情](https://ask.dcloud.net.cn/question/143628)
* 修复 语言服务 html 引用js后不提示js全局变量方法的Bug
* 修复 语言服务 html 输入!+tab后，`<html lang="">`设置为en的Bug [详情](https://ask.dcloud.net.cn/question/143531)
* 修复 语言服务 css属性 属性位置替换文本，替换内容错误的Bug
* 修复 语言服务 Vue script节点，无法提示vue某些代码块的Bug
* 修复 语言服务 Vue script节点，this.方法名，无法转到定义的Bug
* 修复 语言服务 uni-app pages.json提示的文件路径不区分大小写的Bug
* 修复 语言服务 uni-app easycom不规范的写法 导致css class无法提示的Bug [详情](https://ask.dcloud.net.cn/question/143800)
* 修复 撤销、恢复撤销操作，光标位置跳转错误的Bug
* 修复 项目运行过程中，在项目管理器关闭项目可能引发的编辑器闪退的bug
* 修复 App安心打包 某些情况下提交打包失败的Bug
* 修复 App真机运行 某些情况下因adb问题，查找模拟器设备失败的Bug
* 新增 uniCloud 支持云对象本地运行和调试 [详情](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#run-local)
* 【uni-app插件】
  + 新增 vue3 项目内置支持 pinia [详情](https://uniapp.dcloud.net.cn/tutorial/vue3-pinia.html)
  + 修复 3.4.6 版本引发的 vue3 项目使用 pinia 报错的Bug [详情](https://ask.dcloud.net.cn/question/143578)
  + 修复 3.4.6 版本引发的 vue3 项目部分情况编译变慢的Bug [详情](https://github.com/dcloudio/uni-app/issues/3458)
  + App平台、H5平台 修复 canvas 组件画图裁剪异常的Bug [详情](https://ask.dcloud.net.cn/question/142494)
  + App平台、微信小程序平台 新增 vue2 ad-rewarded-video 激励视频广告组件 [详情](https://uniapp.dcloud.net.cn/component/ad-rewarded-video.html)
  + App平台、微信小程序平台 新增 vue2 ad-fullscreen-video 全屏视频广告组件 [详情](https://uniapp.dcloud.net.cn/component/ad-fullscreen-video.html)
  + App平台、微信小程序平台 新增 vue2 ad-interstitial 插屏广告组件 [详情](https://uniapp.dcloud.net.cn/component/ad-interstitial.html)
  + App平台 修复 vue3 nvue 页面引用的静态资源编译后可能不存在的Bug
  + App平台 修复 vue3 nvue 页面事件无法冒泡的Bug
  + App平台 修复 vue3 nvue input，textarea 组件的 v-model 不生效的Bug [详情](https://ask.dcloud.net.cn/question/143547)
  + App平台 修复 navigator 组件 animation-type、animation-duration 属性无效的Bug [详情](https://ask.dcloud.net.cn/question/143377)
  + App平台 修复 vue3 nvue movable 组件使用异常的Bug [详情](https://ask.dcloud.net.cn/question/143742)
  + App平台 修复 3.4.2 版本引发的 ArrayBuffer 类型判断错误的Bug [详情](https://ask.dcloud.net.cn/question/143534)
  + App-Android平台 修复 3.4.6版本 引出的 nvue 页面在部分设备可能出现渲染闪烁的Bug [详情](https://ask.dcloud.net.cn/question/143657)
  + App-Android平台 修复 3.4.6版本 引出的 nvue 页面 boxShadow 在部分情况下可能渲染异常的Bug [详情](https://ask.dcloud.net.cn/question/143727)
  + App-Android平台 修复 bindingx 执行 getComputedStyle 方法返回异常的Bug [详情](https://ask.dcloud.net.cn/question/143697)
  + App-iOS平台 修复 nvue swiper 组件与页面返回手势冲突的Bug [详情](https://ask.dcloud.net.cn/question/137505)
  + H5平台 修复 vue3 项目 html 原生标签（如div）renderjs/wxs 事件监听无法获取 ownerInstance 的Bug [详情](https://github.com/dcloudio/uni-app/issues/3436)
  + H5平台 修复 vue3 项目运行到浏览器，本地服务端口校验可能报错的Bug [详情](https://ask.dcloud.net.cn/question/143504)
  + H5平台 修复 vue3 项目 map 组件 polyline、circles 颜色设置不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3433)
  + 小程序平台 修复 vue3 项目当 style 样式值为数字，部分情况下丢失的Bug [详情](https://github.com/dcloudio/uni-app/issues/3456)
  + 小程序平台 修复 v-if 内连用多个逻辑表达式编译出错的Bug [详情](https://ask.dcloud.net.cn/question/129122)
  + 微信小程序平台 修复 vue3 项目当 input 事件函数返回 Promise 时，输入框显示错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/3462)
  + 微信小程序平台 修复 uni.getSystemInfoSync() 获取的 safeAreaInsets.bottom 为负数的Bug [详情](https://ask.dcloud.net.cn/question/133479)
  + uni-ui 新增 uni-data-select 组件 [详情](https://ext.dcloud.net.cn/plugin?id=7993)
  + uni-ui 新增 uni-breadcrumb 组件 [详情](https://ext.dcloud.net.cn/plugin?id=7992)
  + uni-ui 新增 uni-tooltip 组件 [详情](https://ext.dcloud.net.cn/plugin?id=8020)
* 【uniCloud插件】
  + 修复 云对象 自动展示错误提示界面时 toast 图标错误的Bug [详情](https://ask.dcloud.net.cn/question/142246)
* 【App插件(含5+App和uni-app的App端)】
  + 更新 uni-AD 腾讯优量汇SDK Android为 4.462.1332 版，iOS为 4.13.63 版；今日头条穿山甲SDK iOS为 4.4.0.5 版；快手广告SDK Android为 3.3.23 版，iOS为 3.3.23 版；快手内容联盟SDK iOS为 3.3.28 版；百度百青藤广告SDK iOS为 4.861 版；Sigmob广告联盟SDK iOS为 4.1.0 版
  + Android平台 更新 高德地图SDK为 9.2.0 版， 解决在部分设备使用地图引起应用崩溃的Bug [详情](https://ask.dcloud.net.cn/question/143573)
  + Android平台 修复 uni-AD 离线打包开通开屏广告可能引起应用崩溃的Bug
  + iOS平台 修复 3.4.6版本 引出的 获取底部安全区域高度不正确的Bug [详情](https://ask.dcloud.net.cn/question/143633)
* 【Uni小程序SDK】
  + iOS平台 修复 调用 closeWithCompletion 方法关闭小程序后紧接着在打开小程序可能引起崩溃的Bug

## 3.4.6.20220416-alpha
* 修复 语言服务 uni-app，vue文件，class转到定义，无法转到在App.vue @import引入的公共css文件的Bug
* 修复 语言服务 html文件，引用外部的css文件，当文件地址带有?时，css选择器无法转到定义的Bug
* 修复 语言服务 vue3 API，defineProps、defineExpose，无法提示数据类型的Bug
* 优化 语言服务 vue3，style节点，支持提示:deep、:global
* 修复 语言服务 ts文件，无法提示代码块的Bug
* 调整 markdown一键分享 生成的html文件 调整代码区代码着色
* 修复 3.4.5引出的 当一个文件存在多种换行符时，eslint自动修复替换出错的Bug
* 修复 3.4.0引出的 uni-app 运行 控制台右键菜单点击停止运行，不起作用的Bug
* 【uni-app插件】
  + 优化 vue3 项目 支持导出 onSaveExitState 生命周期 [详情](https://github.com/dcloudio/uni-app/issues/3427)
  + 修复 vue3 项目 错误信息行号可能不正确的Bug [详情](https://ask.dcloud.net.cn/question/143075)
  + App平台 修复 vue3 项目 nvue map 组件部分属性无效的Bug [详情](https://ask.dcloud.net.cn/question/142159)
  + App平台 修复 InnerAudioContext 某些情况下 paused 属性值不正确的Bug [详情](https://ask.dcloud.net.cn/question/141832)
  + App平台 修复 vue3 项目使用 vue-i18n 运行报错的Bug [详情](https://ask.dcloud.net.cn/question/142911)
  + App平台 修复 vue3 项目 renderjs 在低版本手机可能运行报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3366)
  + App-Android平台 修复 uni.saveImageToPhotosAlbum 在部分手机可能无法正常保存到系统相册的Bug [详情](https://ask.dcloud.net.cn/question/143125)
  + App-Android平台 修复 uni.getScreenBrightness 获取屏幕亮度始终返回 -1 的Bug [详情](https://ask.dcloud.net.cn/question/142726)
  + App-Android平台 修复 nvue 页面调用 dom.scrollToElement 滚动到 list 组件指定元素位置可能无效的Bug [详情](https://ask.dcloud.net.cn/question/143035)
  + App-iOS平台 修复 video 不支持 enable-play-gesture 属性的Bug [详情](https://ask.dcloud.net.cn/question/141862)
  + App-iOS平台 修复 nvue input 组件 confirm-hold 属性默认值不正确的Bug
  + App-iOS平台 修复 nvue ad-content-page 显示位置可能偏移的Bug
  + H5平台 修复 input 组件启用 password 后在小米手机钉钉内置浏览器无法弹出键盘的Bug [详情](https://ask.dcloud.net.cn/question/142834)
  + 小程序平台 修复 vue3 项目 pages.json 配置国际化信息显示错误的Bug
  + 小程序平台 修复 vue3 项目在 Windows 系统上生成的依赖文件可能错乱的Bug [详情](https://github.com/dcloudio/uni-app/issues/3425)
  + QQ小程序平台 修复 vue3 项目部分情况运行报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3419)
  + 微信小程序平台 修复 vue3 项目发行为混合分包运行报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3416)
* 【uniCloud插件】
  + 【重要】阿里云 调整 单次数据库查询最大超时时间由1秒调整为3秒，需要重新上传云函数触发更新
  + 【重要】云对象 调整 默认自动显示请求相关ui（等待loading，错误弹框） [详情](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#auto-ui)
  + JQL 修复 部分情况下过度限制了权限的Bug [详情](https://ask.dcloud.net.cn/question/142457)
  + 本地调试插件 修复 HBuilderX 2.4.5 版本引出的部分场景下访问本地云函数误报公共模块冲突的Bug
* 【App插件(含5+App和uni-app的App端)】
  + iOS平台 修复 3.4.5版本 引出的 关闭页面动画异常的Bug [详情](https://ask.dcloud.net.cn/question/142797)
  + iOS平台 修复 音频播放 AudioPlayer 获取暂停状态不准确的Bug [详情](https://ask.dcloud.net.cn/question/141832)
  + iOS平台 修复 音频播放 AudioPlayer 暂停后再恢复播放倍速会重置为1的Bug [详情](https://ask.dcloud.net.cn/question/142848)
  + iOS平台 修复 视频播放控件 video 在刘海屏设备全屏播放时进度条可能无法拖动的Bug [详情](https://ask.dcloud.net.cn/question/141862)
  + iOS平台 修复 视频播放控件 video 设置 show-fullscreen-btn 属性为 false 时可能显示不正确的Bug
* 【Uni小程序SDK】
  + Android平台 新增 支持自定义实现获取匿名设备标识符OAID

## 3.4.5.20220408-alpha
* 优化 语言服务 Vuex commit、dispatch，支持提示mutation、action中的方法
* 修复 语言服务 vue-cli项目 vue文件 script和style标签，输入`lang=`，没有自动拉出相关候选项的Bug
* 修复 语言服务 uni-app vue style节点 import引入文件，以@符号开头的路径，无法转到定义的Bug
* 修复 代码悬浮提示 某些情况下，按下保存，代码悬浮窗口不停变化大小的Bug
* 修复 json文件 引号内回车，自动补充逗号的Bug
* 调整 markdown-share 一键分享 网页内容适配移动端
* 修复 插件API hx.window.getActiveTextEditor replace方法 当同一个文件存在多种换行符时，文本内容替换错误的Bug
* 修复 App真机运行 当HBuilderX语言为英文时，设备选择窗口，窗口内容显示中文的Bug
* 优化 MacOSX App真机运行 运行到iOS模拟器，模拟器选择窗口，支持搜索
* 【uni-app插件】
  + 优化 vue3 项目 支持 vitest 测试框架 [详情](https://github.com/dcloudio/uni-app/issues/3398)
  + 优化 vue3 项目 全平台支持使用 props 接收页面参数 [详情](https://uniapp.dcloud.net.cn/tutorial/migration-to-vue3.html#url-search-params)
  + 修复 vue3 项目 App.vue 中的 provide 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3404)
  + App平台 新增 InnerAudioContext、BackgroundAudioManager 支持倍速播放
  + App平台 修复 vue3 项目 App.vue 中的 css 可能编译报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3403)
  + App平台 修复 uni.getEnv 在 nvue webview 中返回值不准确的Bug [详情](https://uniapp.dcloud.net.cn/component/web-view.html#getenv)
  + App-Android平台 修复 3.4.3版本 引出的 nvue 组件设置 box-shadow 后 border 可能显示异常的Bug
  + App-Android平台 修复 3.4.3版本 引出的 tabBar 设置 iconPath 且未设置 selectedIconPath 可能引起图标无法正常显示的Bug
  + App-Android平台 修复 nvue 页面 flex 布局在部分设备可能出现换行计算不正确的Bug
  + App-iOS平台 修复 在页面生命周期 onLoad 方法中调用 lockOrientation 锁定屏幕方向可能引起布局异常的Bug
  + App-iOS平台 修复 3.4.4版本 引出的 tabBar 图标显示错位的Bug [详情](https://ask.dcloud.net.cn/question/142685)
  + H5平台 修复 vue3 项目同时使用 style 节点和 style scoped 节点时，样式可能错乱的Bug [详情](https://github.com/dcloudio/uni-app/issues/3410)
  + 小程序平台 优化 vue3 项目支持动态导入静态资源 [详情](https://github.com/dcloudio/uni-app/issues/3376)
  + 小程序平台 修复 vue3 项目 slot 在部分复杂情况运行报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3346)
  + 小程序平台 修复 vue2 项目 v-if 中同时包含成员表达式和逻辑表达式编译出错的Bug [详情](https://ask.dcloud.net.cn/question/142293)
  + 微信小程序平台 优化 uni.showActionSheet 支持 title 参数
  + 支付宝小程序平台 修复 vue3 项目部分情况下渲染错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/3408)
* 【uniCloud插件】
  + 修复 3.4.4版本 引出的 clientDB 本地运行报错的Bug
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 修复 uni-AD 腾讯优量汇插屏广告在 onLoad 回调中执行 show 可能引起广告无法正常显示的Bug
  + iOS平台 修复 安心打包使用 swift 开发的uni原生插件时上传 AppStore 报`ITMS-90426: Invalid Swift Support`错误的Bug [详情](https://ask.dcloud.net.cn/question/142611)
  + iOS平台 修复 在 iOS15.4 及以上设备系统时间设置为12小时制 pickDate 返回值异常的Bug [详情](https://ask.dcloud.net.cn/question/141906)

## 3.4.4.20220403-alpha
* 修复 语言服务 vue 使用this.访问data中定义的数据对象，this.xx. 没有根据数据类型，提示相应方法的Bug
* 修复 语言服务 vue 模板语法`{{}}`内，使用js表达式，回车后没有自动补充`()`的Bug
* 修复 语言服务 css 代码助手候选项 !important 重复显示的Bug
* 修复 语言服务 uni-app vue 代码助手候选项 picker-view 重复显示的Bug
* 修复 语言服务 uni-app pages.json 某些属性没有提示的Bug
* 修复 语言服务 uni-app cli项目，uni.开头的api, 回车后`()`内没有补充`{}`的Bug
* 修复 语言服务 uni-app vue3项目，`import {} from "@dcloudio/uni-app"`, `{}`内无法提示uni-app生命周期方法的Bug
* 优化 语言服务 uni-app vue文件 import引入文件 支持提示以@符号开头的路径
* 优化 语言服务 vue 支持提示ref和$refs关键字
* 优化 代码悬浮提示 减少不要的悬浮提示
* 修复 MacOSX 某些情况下，HBuilderX启动后，立即按下`command+w`关闭标签卡，编辑器闪退的Bug
* 优化 App真机运行 运行到iOS模拟器，设备选择窗口，将上一次使用的模拟器放置在第一条
* 优化 App真机运行 运行到iOS设备，运行失败时的控制台提示语
* 优化 App真机运行 运行到Android，获取设备，对用户自定义adb路径，增加有效性检查
* 修复 3.4.0引出的 apk、ipa文件，右键菜单，安装到手机，没有显示手机设备列表的Bug
* 修复 3.4.0引出的 App真机运行 Windows 32系统，运行App项目到iOS、Android，无法查找到设备的Bug
* 修复 3.4.0引出的 App真机运行 在【设置 - 运行设置】中，自定义的模拟器端口，没有生效的Bug
* 修复 3.4.0引出的 App真机运行 Windows 运行App项目到夜神模拟器，真机运行过程中，模拟器设备断开连接的Bug
* 修复 3.4.0引出的 App真机运行 adb connect连接Android真机，真机运行过程中，手机设备断开连接的Bug
* 修复 3.4.0引出的 App真机运行 uni-app 运行到iOS/Android，设备选择窗口，某些情况下，一直显示正在获取的Bug
* 修复 3.4.0引出的 App真机运行 MacOSX 运行项目到iOS模拟器，某些情况下，选择设备与实际运行设备不一致的Bug
* 修复 uni-app 新建页面，输入已存在的页面名称，不勾选创建同名目录，旧文件被覆盖的Bug
* 【uni-app插件】
  + App平台、H5平台 新增 input 组件配置 ignoreCompositionEvent 属性 [详情](https://uniapp.dcloud.io/component/input?id=input)
  + App平台 新增 tabbar 支持配置 iconfont [详情](https://uniapp.dcloud.net.cn/api/ui/tabbar?id=settabbaritem)
  + App平台 修复 vue2 nvue 页面文本首尾回车符占用高度的Bug [详情](https://ask.dcloud.net.cn/question/95429)
  + App平台 修复 vue3 项目 uni.getSavedFileList、uni.getSavedFileInfo、uni.removeSavedFile、uni.getFileInfo 无效的Bug  [详情](https://ask.dcloud.net.cn/question/142428)
  + App-Android平台 修复 nvue list 组件横向滚动不会触发 loadmore 事件的Bug
  + App-Android平台 修复 连续调用 uni.chooseImage 在部分手机可能引起应用闪退的Bug
  + App-Android平台 修复 3.4.3 引出的 tabBar 的列表项未设置 iconPath 会导致文字显示不全的Bug [详情](https://ask.dcloud.net.cn/question/142250)
  + App-iOS平台 修复 video 组件 vslide-gesture-in-fullscreen 属性无效的Bug [详情](https://ask.dcloud.net.cn/question/138299)
  + App-iOS平台 修复 nvue image 组件不支持 gif 图片中设置循环次数参数的Bug [详情](https://ask.dcloud.net.cn/question/140176)
  + 小程序平台 修复 vue3 项目 v-model.number 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3381)
  + 小程序平台 修复 vue3 项目页面复杂时可能编译报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3397)
  + 微信小程序平台 修复 vue3 项目 input 事件 return 一个字符串没有同步到输入框的Bug [详情](https://github.com/dcloudio/uni-app/issues/3371)
  + 百度小程序平台 修复 vue3 项目 onInit 生命周期不触发的Bug [详情](https://github.com/dcloudio/uni-app/issues/3384)
  + 支付宝小程序平台 修复 vue2 项目插件内组件部分事件不触发的Bug [详情](https://ask.dcloud.net.cn/question/142048)
  + 支付宝小程序平台 修复 vue3 项目 默认分享功能失效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3377)
* 【uniCloud插件】
  + 修复 3.4.0版本引出的云函数子目录内文件引用公共模块失败的Bug
* 【App插件(含5+App和uni-app的App端)】
  + 新增 音频播放 AudioPlayer 支持 playbackRate 设置倍速播放 [文档](https://www.html5plus.org/doc/zh_cn/audio.html#plus.audio.AudioPlayer.playbackRate)
  + Android平台 更新 高德定位SDK为 6.0.1 版，高德地图SDK为 9.0.1 版；UniPush 使用的个推SDK为 3.2.9.0 版，小米厂商推送库SDK为 3.1.1 版；Google地图SDK为 18.0.2 版
  + Android平台 优化 二维码扫码检测到 QR 码时自动放大，提升扫码识别率 [详情](https://ask.dcloud.net.cn/question/142209)
  + 【重要】Android平台 修复 uni-AD 穿山甲广告联盟在部分设备可能提示`应用的uni-AD业务状态异常`的Bug
  + iOS平台 修复 视频播放控件 video 播放视频音量与系统音量不一致的Bug

## 3.4.3.20220325-alpha
* 新增 HBuilderX CLI uni-app 制作应用wgt包 [详情](https://hx.dcloud.net.cn/cli/publish-app-wgt)
* 新增 HBuilderX CLI uni-app 生成本地打包App资源 [详情](https://hx.dcloud.net.cn/cli/publish-app-appResource)
* 新增 代码悬浮提示 支持着色
* 新增 语言服务 manifest.json settings.json支持代码提示
* 优化 语言服务 javaScript 代码提示
* 修复 语言服务 css变量 转到定义时，下划线绘制错误的Bug
* 修复 语言服务 vue文件 `import ... from ...`，无法提示文件路径的Bug
* 修复 语言服务 uni-app uni.navigateTo()等页面跳转到方法，url无法提示页面的Bug
* 修复 语言服务 某些情况下，在图片上转到定义导致HBuilderX崩溃的Bug
* 修复 分栏 某些情况下，打开同一份文档时，关掉第一个文档窗口崩溃的Bug
* 调整 编辑器 vue文件 async类关键字颜色
* 修复 原生App-云打包 项目过大时导致无法提交到云端打包的Bug
* 优化 uni-app 发行 制作应用wgt包窗口样式
* 优化 uniCloud 新建公共模块界面 支持选择模板
* 【uni-app插件】
  + 【重要】App平台 nvue 页面支持 vue3（需要项目的 Vue 版本切换为3）[详情](https://uniapp.dcloud.net.cn/tutorial/migration-to-vue3.html)
  + App平台、H5平台 新增 map 组件支持 polygons [详情](https://uniapp.dcloud.io/component/map)
  + App平台、小程序平台 修复 vue3 项目配置 base 后资源路径可能错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/3362)
  + App平台 新增 打开微信客服功能 [详情](https://uniapp.dcloud.io/api/plugins/share.html)
  + App平台 修复 vue3 项目内联样式引用静态资源可能错误的Bug [详情](https://ask.dcloud.net.cn/question/141278)
  + App平台 新增 nvue ad-content-page 组件支持内容播放状态事件start、pause、resume、complete [规范](https://uniapp.dcloud.io/component/ad-content-page.html#%E7%9F%AD%E8%A7%86%E9%A2%91%E5%86%85%E5%AE%B9%E8%81%94%E7%9B%9F%E7%BB%84%E4%BB%B6)
  + App-Android平台 优化 nvue 组件 box-shadow 渲染逻辑，解决在部分设备可能出现排版异常及闪烁的问题 [详情](https://uniapp.dcloud.io/tutorial/nvue-css.html#android-box-shadow)
  + App-Android平台 修复 nvue swiper 组件设置 circular 为 true 时首次启动可能先显示最后一项的Bug [详情](https://ask.dcloud.net.cn/question/140931)
  + App-Android平台 修复 nvue swiper 组件在特定环境下可能出现页面空白的Bug [详情](https://ask.dcloud.net.cn/question/140942)
  + App-iOS平台 修复 nvue swiper 组件内嵌 list-waterfall 时，横向滑动的同时列表还可以竖向滚动的Bug [详情](https://ask.dcloud.net.cn/question/134909)
  + App-iOS平台 修复 nvue 页面内存在可滚动子组件时，开启 enablePullDownRefresh 下拉刷新功能无效的Bug
  + App平台 修复 vue3 组件 picker-view 调整列数据时渲染错误的Bug [详情](https://ask.dcloud.net.cn/question/140609)
  + H5平台 修复 vue3 项目配置 base 发行后资源路径可能错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/3354)
  + 小程序平台 优化 vue3 项目自定义组件支持 v-bind="" 语法 [详情](https://github.com/dcloudio/uni-app/issues/3330)
  + QQ小程序平台 修复 vue3 项目 appid 配置不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3339)
  + 字节跳动小程序平台 修复 vue3 项目部分情况下数据不响应的Bug [详情](https://github.com/dcloudio/uni-app/issues/3340)
  + 字节跳动小程序平台 修复 vue3 项目 options 方式配置 provide/inject 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3360)
  + 支付宝小程序平台 修复 vue3 项目分包页面事件响应不正常的Bug [详情](https://ask.dcloud.net.cn/question/140742)
* 【uniCloud插件】
  + 修复 公共模块右键管理依赖的公共模块不生效的Bug
  + 修复 修复本地运行云函数调用云对象报错的Bug
* 【App插件(含5+App和uni-app的App端)】
  + uni-AD 新增 百度百青藤广告联盟支持信息流广告
  + Android平台 更新 uni-AD 百度百青藤广告SDK 为 9.202 版
  + Android平台 修复 在部分设备识别国际化语言不正确的Bug [详情](https://ask.dcloud.net.cn/question/141688)
* 【Uni小程序SDK】
  + Android平台 修复 微信登录连续多次调用可能会导致失败的Bug
  + Android平台 修复 转场动画在 Android12 设备可能失效的Bug
  + Android平台 修复 调用 startActivityForUniMPTask 在 Android8 以下设备可能会引起应用崩溃的Bug

## 3.4.2.20220310-alpha
* 修复 3.4.0引出的 打开失去焦点自动保存，多文件字符搜索，点击搜索结果后文件内容被覆盖的Bug [详情](https://ask.dcloud.net.cn/question/140782)
* 修复 3.4.0引出的 Wap2App项目，无法提交打包的Bug [详情](https://ask.dcloud.net.cn/question/140700)
* 修复 3.4.0引出的 Android真机运行 没有使用设置中用户自定义adb的Bug
* 修复 代码格式化，撤销操作，光标位置错误的Bug [详情](https://ask.dcloud.net.cn/question/140970)
* 修复 某些情况下，插件安装后，插件状态不对的Bug
* 修复 App 安心打包 manifest.json 配置Google统计 安心打包没有提交相关文件的bug
* 修复 语言服务 html行内标签, `=`后面存在空格时，无法正确提示CSS代码的Bug
* 修复 语言服务 uni-app easycom 组件名称提示错误的Bug
* 修复 语言服务 vue文件 hover 和 resolve 时提示内容缺失的Bug
* 修复 语言服务 CSS代码提示 某些情况下，font-family提示错误的Bug
* 修复 语言服务 CSS代码提示 rgb、rgba等函数补全错误的Bug
* 【uni-app插件】
  + App平台 新增 vue 页面支持 live-pusher 组件 [详情](https://uniapp.dcloud.net.cn/component/live-pusher)
  + App平台 修复 uni.request、uni.onSocketMessage 等接口返回的 ArrayBuffer 类型不可用 instanceof 做类型判断的Bug
  + App平台 修复 vue3 项目 wxs/renderjs 监听事件运行报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3324)
  + App-Android平台 修复 nvue map组件使用高德地图时，频繁调用 addMarkers 增加聚合点可能引起崩溃的Bug [详情](https://ask.dcloud.net.cn/question/140461)
  + App-Android平台 修复 nvue map组件使用谷歌地图时，调用 moveAlong 移动 marker 可能出现偏移的Bug
  + App-iOS平台 补齐 uni-AD 支持 nvue ad-content-page组件 [文档](https://uniapp.dcloud.net.cn/component/ad-content-page.html#%E7%9F%AD%E8%A7%86%E9%A2%91%E5%86%85%E5%AE%B9%E8%81%94%E7%9B%9F%E7%BB%84%E4%BB%B6)
  + App-iOS平台 修复 nvue 组件 userInteractionEnabled 属性无效的Bug [详情](https://ask.dcloud.net.cn/question/140838)
  + App-iOS平台 修复 nvue refresh 组件 pullingdown 事件触发时机不正确的Bug [详情](https://ask.dcloud.net.cn/question/138962)
  + H5平台 修复 vue3 项目 wxs/renderjs 热刷新不生效的Bug [详情](https://ask.dcloud.net.cn/question/140800)
  + H5平台 修复 vue3 项目特定情况下拉刷新后页面跳转的Bug [详情](https://github.com/dcloudio/uni-app/issues/3326)
  + 小程序平台 修复 vue3 项目模板中 style 属性包含换行符时编译报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3320)
  + 支付宝小程序平台 优化 vue3 项目默认开启 es6=>es5 [详情](https://ask.dcloud.net.cn/question/140742)
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 新增 Google支付支持 isReadyToPay 方法 [文档](https://www.html5plus.org/doc/zh_cn/payment.html#plus.payment.PaymentChannel.isReadyToPay)

## 3.4.1.20220308-alpha
* 修复 3.4.0引出的 uni-app 新建页面，修改pages.json内容，导致编辑器闪退的Bug [详情](https://ask.dcloud.net.cn/question/140732)
* 【uni-app插件】
  + App平台 修复 uni.getBackgroundAudioManager 的 onPrev onNext 事件无效Bug [详情](https://ask.dcloud.net.cn/question/107325)
  + App平台 修复 3.4.0 引发的 vue2 项目 canvas 组件 fillText 失效的Bug [详情](https://ask.dcloud.net.cn/question/140786)
  + App平台 修复 3.4.0 引发的 vue2 项目 nvue 页面的 uni.createLivePusherContext 无效Bug [详情](https://ask.dcloud.net.cn/question/140743)
  + App平台 修复 vue3 项目 navigator 组件和 rich-text 组件嵌套使用时 scopeId 值不一致导致的样式Bug [详情](https://ask.dcloud.net.cn/question/140644)
  + App-iOS平台 修复 nvue map 组件 marker 的 joinCluster 为 false 时 removeMarkers 方法不生效的Bug [详情](https://ask.dcloud.net.cn/question/140648)
  + App-iOS平台 修复 nvue rich-text 组件 text-overflow 样式不生效的Bug [详情](https://ask.dcloud.net.cn/question/140586)
  + H5平台 修复 部分情况下 input 组件显示数值错误的Bug [详情](https://ask.dcloud.net.cn/question/140366)
  + 小程序平台 修复 vue3 项目部分情况下视图更新延迟的Bug [详情](https://github.com/dcloudio/uni-app/issues/3311)
* 【App插件(含5+App和uni-app的App端)】
  + Android平台 3.4.0 引出的 UniPush模块使用 Oppo 厂商通道时云端打包失败的Bug [详情](https://ask.dcloud.net.cn/question/140765)
* 【Uni小程序SDK】
  + iOS平台 修复 小程序SDK中设置 user-agent 影响宿主原生页面中 Webview 的Bug

## 3.4.0.20220304-alpha
* 【重要】调整 HBuilderX语言服务 由Java切换为Node，减少内存占用、增强语法提示
* 新增 新建uni-app项目时直接选择Vue2或3的版本（后续可在manifest里调整）
* 新增 文档保存时自动格式化，可通过【设置】-【编辑器配置】-【保存时自动格式化】开启
* 【调整】 App真机运行 不再长期监听手机，运行时检测，减少资源消耗
* 修复 文档格式化后，撤销时光标位置不对的Bug
* 修复 某些情况，Git更新文件后，编辑器内文件不会自动刷新的Bug
* 修复 查找索引符号 搜索后，HBuilderX闪退的Bug
* 修复 某些情况，文档编辑后出现着色错乱的Bug
* 修复 uni-app manifest.json中app-plus-compilerVersion未配置时发行和运行会弹出设置微信开发者工具对话框的Bug
* 修复 uni-app manifest 生成通用链接时，协作者选择服务空间时获取不到自定义域名的Bug
* 调整 安装HBuilderX核心插件时，由下载最新版插件调整为和当前HBuilderX版本匹配的插件
* 优化 uni-app 运行菜单和发行小程序的界面样式
* 【uni-app插件】
  + 新增 vue2 项目支持发布到 京东小程序
  + 修复 vue3 项目兼容 vite@2.8.x [详情](https://ask.dcloud.net.cn/question/139311)
  + 修复 vue3 项目兼容 vite-plugin-eslint [详情](https://github.com/dcloudio/uni-app/issues/3247)
  + App平台、H5平台 优化 取消全局 canvas 高清处理，支持配置单个 canvas 组件 hidpi 属性
  + App平台、H5平台 修复 自定义组件监听 tap.native 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3259)
  + App平台、H5平台 修复 vue3 项目 uni.pageScrollTo 的 duration 为0时不生效的Bug [详情](https://ask.dcloud.net.cn/question/139432)
  + App平台、H5平台 修复 vue3 项目 input 组件类型为 number 时在低版本 webview 失去焦点时报错的Bug [详情](https://ask.dcloud.net.cn/question/138088)
  + App平台 新增 地图支持 Google地图 [详情](https://uniapp.dcloud.net.cn/app-maps)
  + App平台 新增 支付支持 Paypal、Stripe、Google Pay [详情](https://uniapp.dcloud.io/app-payment-paypal)
  + App平台 新增 登录支持 Google、Facebook [详情](https://uniapp.dcloud.io/api/plugins/login?id=app-oauth)
  + App平台 新增 vue 页面 video 组件支持 vslide-gesture、vslide-gesture-in-fullscreen 属性 [详情](https://uniapp.dcloud.io/component/video)
  + App平台 新增 pages.json 支持在 style 配置 disableSwipeBack 以禁用 iOS 侧滑返回
  + App平台 修复 uni.addPhoneContact 重复添加联系人的Bug [详情](https://gitee.com/dcloud/uni-app/issues/I4NY6C)
  + App平台 修复 vue3 项目使用 html 原生标签（如div）时，事件监听报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3240)
  + App-Android平台 修复 nvue image 组件 mode 属性设置为 widthFix/HeightFix 时可能导致图片无法显示的Bug [详情](https://ask.dcloud.net.cn/question/139541)
  + App-Android平台 修复 nvue list 组件插入列表项可能引起页面闪烁的Bug [详情](https://ask.dcloud.net.cn/question/139424)
  + App-Android平台 修复 nvue web-view 组件 progress 颜色值不支持3位十六进制格式字符串的Bug [详情](https://ask.dcloud.net.cn/question/138670)
  + App-Android平台 修复 nvue web-view 组件 无法正常加载使用非受信任证书网页的Bug [详情](https://ask.dcloud.net.cn/question/134287)
  + App-Android平台 修复 nvue animation 动画切到后台可能无法执行的Bug [详情](https://ask.dcloud.net.cn/question/137868)
  + App-Android平台 修复 nvue map 组件 marker 设置 joinCluster 为 true 时导致 callouttap 事件不响应的Bug [详情](https://ask.dcloud.net.cn/question/136381)
  + App-Android平台 修复 nvue text 组件 font-style 设置 italic 在部分设备可能无效的Bug [详情](https://ask.dcloud.net.cn/question/120801)
  + App-Android平台 修复 nvue 页面切换可能导致 plus.key.addEventListener 监听 keydown 事件不触发回调的Bug [详情](https://ask.dcloud.net.cn/question/140203)
  + App-iOS平台 修复 vue3 项目 调试时启动白屏的Bug
  + H5平台 优化 vue3 项目 navigator 组件使用 a 标签渲染以利于SEO
  + H5平台 修复 vue3 项目 html 中引入 static 目录的 js 文件包含 ifdef 编译报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3201)
  + H5平台 修复 vue3 项目 renderjs 发行后不正常的Bug [详情](https://ask.dcloud.net.cn/question/137832)
  + H5平台 修复 vue3 项目 dataset 不支持对象类型错误的Bug [详情](https://ask.dcloud.net.cn/question/139181)
  + H5平台 修复 vue3 项目 禁用摇树后，uni.showModal 等弹窗缺少样式的Bug [详情](https://ask.dcloud.net.cn/question/139593)
  + H5平台 修复 vue3 项目 热刷新编译报错的Bug [详情](https://ask.dcloud.net.cn/question/135765)
  + H5平台 修复 vue3 项目 text 组件使用 v-if 时显示错误的Bug [详情](https://github.com/dcloudio/uni-app/issues/3225)
  + H5平台 修复 map 组件 marker 不能设置 id 为 0 的Bug
  + 小程序平台 修复 vue3 项目 uni.getSystemInfo 无法获取 deviceId 的Bug [详情](https://ask.dcloud.net.cn/question/139733)
  + 小程序平台 修复 vue3 项目 不支持 v-html 的Bug [详情](https://ask.dcloud.net.cn/question/138290)
  + 小程序平台 修复 vue3 项目 v-if 中使用 wxs 等模块时报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3199)
  + 小程序平台 修复 vue3 项目 defineEmits 事件名包含 - 分隔符时无法正常监听的Bug [详情](https://github.com/dcloudio/uni-app/issues/3210)
  + 小程序平台 修复 vue3 项目 setup 手动引入组件不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3213)
  + 小程序平台 修复 vue3 项目 v-for 嵌套使用时部分情况运行报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3263)
  + 小程序平台 修复 vue3 项目 wxs 调用 callMethod 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3218)
  + 小程序平台 修复 vue3 项目 全局组件路径解析错误的Bug [详情](https://ask.dcloud.net.cn/question/138662)
  + 小程序平台 修复 vue3 项目 全局 mixin 分享 onShareAppMessage，onShareTimeline 不生效的Bug [详情](https://ask.dcloud.net.cn/question/140351)
  + 微信小程序平台 修复 vue2 项目 v-for 遍历部分表达式时 stop 修饰符无效的Bug [详情](https://ask.dcloud.net.cn/question/138684)
  + 微信小程序平台 修复 vue3 项目 canvas 监听 touch 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3209)
  + 微信小程序平台 修复 vue3 项目部分情况下事件监听错乱的Bug [详情](https://github.com/dcloudio/uni-app/issues/3228)
  + 微信小程序平台 修复 vue3 项目使用小程序插件组件无法传递属性的Bug [详情](https://github.com/dcloudio/uni-app/issues/3257)
  + 支付宝小程序平台 修复 vue2 项目小程序组件事件监听失效的Bug [详情](https://github.com/dcloudio/uni-app/issues/2273)
  + 支付宝小程序平台 修复 vue2 项目小程序插件中组件事件监听失效的Bug [详情](https://github.com/dcloudio/uni-app/issues/2410)
  + 【重要】hello uniCloud 新增云对象基础使用示例[详情](https://ext.dcloud.net.cn/plugin?id=4082)
* 【uniCloud】
  + 【重要】新增`云对象`。将callfunction函数调用升级为模块化方式，网络不再传递json，前端对象化使用云API [详情](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj)
  + 【调整】发送短信API 从内置库剥离为扩展库 uni-cloud-sms [详情](https://uniapp.dcloud.net.cn/uniCloud/send-sms?id=extension)
  + 【调整】一键登录API 从内置库剥离为扩展库 uni-cloud-verify [详情](https://uniapp.dcloud.net.cn/uniCloud/univerify?id=extension)
  + 【调整】uniCloud本地调试插件 云函数右键本地运行时，此云函数内的callFunction由调用云端云函数改为调用本地云函数
  + 新增 jql语法 允许在 getTemp 联表查询的虚拟联表内使用 groupBy distinct [详情](https://uniapp.dcloud.net.cn/uniCloud/jql?  id=lookup-with-temp)
  + 优化 HBuilderX新建云函数的界面支持选择模板和依赖
  + 修复 阿里云 云函数删除文件接口返回数据格式不正确的Bug
  + 修复 uni-cloud-jql扩展库 权限校验失败等场景未抛出错误的Bug
* 【App插件(含5+App和uni-app的App端)】
  + 新增 支持Google地图 [详情](https://uniapp.dcloud.io/app-maps?id=google%e5%9c%b0%e5%9b%be)
  + 【重要】uni-AD 新增 百度百青藤广告联盟 支持开屏、插屏、激励视频广告 [详情](https://ask.dcloud.net.cn/article/36769)
  + 【重要】Android平台 新增 uni-AD 支持华为广告联盟 包括开屏、信息流、插屏、激励视频广告 [详情](https://ask.dcloud.net.cn/article/36769)
  + Android平台 更新 UniPush 使用的个推SDK版本为3.2.7.0，个推核心组件SDK版本为3.1.7.0，优化云端打包按需包含厂商通道SDK
  + Android平台 优化 应用启动首页可能出现上下抖动的Bug [详情](https://ask.dcloud.net.cn/question/138243)
  + Android平台 修复 使用 X5 内核调用 plus.key.addEventListener 监听 keyup 事件不触发回调的Bug
  + Android平台 修复 Android8及以上设备 plus.navigator.createShortcut 无法创建桌面快捷图标的Bug [详情](https://ask.dcloud.net.cn/question/125119)
  + Android平台 修复 视频播放控件 video 边缘可能出现黑线的Bug [详情](https://ask.dcloud.net.cn/question/138320)
  + Android平台 修复 在部分设备调用 plus.runtime.restart 可能引起应用闪退的Bug [详情](https://ask.dcloud.net.cn/question/138965)
  + Android平台 修复 系统语言设置为土耳其语时，tabbar 切换选项可能导致不显示的Bug [详情](https://ask.dcloud.net.cn/question/139313)
  + Android平台 修复 本地相册选择视频设置 compressed 为 false 时依然会压缩的Bug [详情](https://ask.dcloud.net.cn/question/140417)
  + iOS平台 新增 uni原生插件支持 applicationMain 获取 main 函数启动参数 argc、argv [文档](https://nativesupport.dcloud.net.cn/NativePlugin/course/ios?id=hook%e7%b3%bb%e7%bb%9f%e4%ba%8b%e4%bb%b6)
  + iOS平台 修复 Webview窗口标题栏 titleNView无法动态更新网络页面标题的Bug [详情](https://ask.dcloud.net.cn/question/138958)
  + iOS平台 修复 compressVideo 视频压缩可能出现尺寸错乱的Bug [详情](https://ask.dcloud.net.cn/question/138303)
  + iOS平台 修复 微博分享 type 为 web 时无法正常分享的Bug [详情](https://ask.dcloud.net.cn/question/138830)
  + iOS平台 修复 播放背景音频时系统锁屏界面音乐播放器的进度条可能显示不正确的Bug [详情](https://ask.dcloud.net.cn/question/140101)
* 【uni小程序SDK】
  + Android平台 优化 混淆配置规则，解决 zip4j 可能与其他的库冲突的Bug
  + Android平台 修复 3.3.5 引出的 微信支付回调可能会引起崩溃的Bug
  + Android平台 修复 多个小程序分别配置使用 vue2、vue3， 同时打开可能引起白屏的Bug [详情](https://ask.dcloud.net.cn/question/138576)
  + Android平台 修复 关闭小程序后台运行模式，重复操作打开/关闭小程序可能导致小程序无法正常运行的Bug
  + Android平台 修复 小程序切换到后台，直达页面启动时出现闪屏的Bug
  + iOS平台 修复 关闭小程序后快速启动小程序并直达页面，重复操作偶现崩溃的Bug

## 3.3.12.20220222-alpha
* 修复 HBuilderX CLI发行微信小程序，某些情况下，HBuilderX出现出现闪退的Bug [详情](https://ask.dcloud.net.cn/question/139189)
* 【uni-app插件】
  + App平台、H5平台 修复 vue3 项目两个开启了下拉刷新的页面跳转后返回，下拉刷新不触发 onPullDownRefresh 生命周期的Bug [详情](https://github.com/dcloudio/uni-app/issues/3187)
  + App平台 修复 vue3 项目 nvue 页面使用 map 组件时部分方法不生效的Bug [详情](https://ask.dcloud.net.cn/question/138515)
  + App-Android平台 修复 picker 组件选择选项后同页面 input 组件可能无法正常获取焦点的Bug [详情](https://ask.dcloud.net.cn/question/138237)
  + App-Android平台 修复 vue3 项目 安卓低版本时使用 type=number 的 input 组件输入报错的Bug [详情](https://ask.dcloud.net.cn/question/138088)
  + App-iOS平台 修复 3.3.2 版本引出的支持多个音频同时播放引发iOS影响静音开关的问题，默认不支持同时播放多个文件，如果需要可手动设置 sessionCategory
  + App-iOS平台 修复 vue3 项目 canvas 组件绘制本地图像后无法导出到本地到Bug
  + H5平台 优化 uni.chooseLocation 支持传入坐标
  + H5平台 修复 vue2 项目开启摇树后 ad 组件失效的Bug
  + H5平台 修复 vue3 项目 image 组件 mode=heightFix 图像大小显示错误的Bug
  + H5平台 修复 vue3 项目 button 组件发行后 loading 不显示的Bug
  + 支付宝小程序平台 修复 触发自定义事件报错的Bug [详情](https://ask.dcloud.net.cn/question/138706)
* 【uniCloud】
  + 修复 JQL语法 getTemp 返回结果传递给组件属性时在微信小程序端报错的Bug [详情](https://ask.dcloud.net.cn/question/138308)
* 【App插件(含5+App和uni-app的App端)】
  + 更新 uni-AD 腾讯优量汇SDK Android为 4.450.1320 版，iOS为 4.13.50 版；今日头条穿山甲SDK Android为 4.3.0.1 版， iOS为 4.3.0.2 版；快手广告SDK Android为 3.3.21 版，iOS为 3.3.21 版
  + Android平台 修复 一键登录 授权页面服务协议自定义复选框状态图片设置不正确的Bug [详情](https://ask.dcloud.net.cn/question/139830)
  + iOS平台 修复 Downloader 下载图片文件可能失败的Bug [详情](https://ask.dcloud.net.cn/question/116101)
  + iOS平台 修复 geitImageInfo 可能不触发回调的Bug [详情](https://ask.dcloud.net.cn/question/139361)
* 【uni小程序SDK】
  + iOS平台 修复 动态切换横竖屏导致页面布局异常的Bug

## 3.3.8.20220114-alpha
* 修复 MacOSX 3.3.7-alpha引出的 uniCloud虚拟目录，点击后提示没有权限的Bug
* 【uniCloud】
  + 修复 3.3.7-alpha引出的JQL数据库管理无法正常使用的Bug [详情](https://ask.dcloud.net.cn/question/138139)
* 【uni-app插件】
  + App-Android平台 修复 3.3.7 版本引出的 nvue list 组件滚动后也会触发 click 事件的Bug
  + 小程序平台 修复 vue3 项目 组件使用 id 属性不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3179)
  + 小程序平台 修复 vue3 项目 部分情况 defineExpose 不生效的Bug [详情](https://github.com/dcloudio/uni-app/issues/3180)
  + 小程序平台 修复 vue3 项目 兼容 unocss 插件 [详情](https://ask.dcloud.net.cn/question/138021)
  + 微信小程序平台 修复 vue3 项目 当 v-for 循环变量名为 index 时渲染不正确的Bug [详情](https://github.com/dcloudio/uni-app/issues/3193)
  + 微信小程序平台 修复 vue3 项目无法自动开启开发工具窗口的Bug
  + 支付宝小程序平台 修复 vue3 项目 mixin 中包含 props 运行报错的Bug [详情](https://github.com/dcloudio/uni-app/issues/3191)

## 3.3.7.20220112-alpha
* 新增 HBuilderX CLI 支持发行uni-app到微信小程序 [详情](https://hx.dcloud.net.cn/cli/publish-mp-weixin)
* 新增 HBuilderX CLI 支持发行uni-app到H5 [详情](https://hx.dcloud.net.cn/cli/publish-h5)
* 修复 MacOSX 某些情况下，项目管理器项目无法展开的Bug
* 调整 内置浏览器 地理位置设置 经纬度支持设置6位小数
* 修复 App 真机运行 部分Windows电脑运行App到iOS15以上手机失败的Bug
* 修复 App 真机运行 部分Android 11系统，同步文件失败的Bug
* 修复 uni-app 安心打包 没有生成iOS符号表文件的Bug
* 调整 uni-app 发行到微信小程序，支持自动上传代码到微信平台，无需再通过微信开发者工具上传发行 [详情](https://hx.dcloud.net.cn/Tutorial/App/uni-app-publish-mp-weixin)
* 【uni-app插件】
  + App平台、H5平台 新增 textarea、input 组件支持 confirm-hold 属性 [详情](https://uniapp.dcloud.io/component/input)
  + App平台、H5平台 优化 image 组件 draggable 属性默认值改为 false
  + App平台 优化 uni.request 请求参数支持 ArrayBuffer 类型
  + App平台 修复 vue3 项目 发行后 renderjs 调用 ownerInstance.callMethod 失效的Bug [详情](https://ask.dcloud.net.cn/question/137832)
  + App平台 修复 vue3 项目 picker 组件默认语言固定为英文的Bug [详情](https://ask.dcloud.net.cn/question/136954)
  + App-Android平台 修复 nvue input 组件不支持自定义字体的Bug [详情](https://ask.dcloud.net.cn/question/135514)
  + App-Android平台 修复 nvue list 组件不支持 click 事件的Bug [详情](https://ask.dcloud.net.cn/question/136754)
  + App-iOS平台 修复 nvue swiper-list 组件滚动条无法隐藏的Bug [详情](https://ask.dcloud.net.cn/question/136261)
  + H5平台 修复 右键单击事件 contextmenu 丢失 clientX、clientY 属性的Bug [详情](https://ask.dcloud.net.cn/question/136530)
  + 小程序平台 修复 模板中包含转义引号时在小程序开发工具中编译报错或显示异常的Bug
  + 微信小程序平台 修复 多页面，组件内使用插槽数据时，差量编译丢失插槽信息的Bug [详情](https://ask.dcloud.net.cn/question/136258)
* 【uniCloud】
  + 新增 JQL语法 使用 getTemp 进行联表查询时，支持在临时表内使用 as 或其他运算操作 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql?id=lookup-with-temp)
  + 新增 JQL语法 使用 getTemp 进行联表查询时，支持在虚拟联表内使用 foreignKey 方法指定要使用的 foreignKey 的归属的字段 [详情](https://uniapp.dcloud.net.cn/uniCloud/jql?id=lookup-with-temp)
  + 新增 web控制台 阿里云 前端网页托管支持为指定路径开启 uni-app history 路由跳转模式支持 [详情](https://uniapp.dcloud.net.cn/uniCloud/hosting?id=routing)
  + 新增 uni-id 支持自定义国际化语言支持 [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id?id=custom-i8n)
  + 修复 uni-id 一键登录时未校验重复手机号是否已验证的Bug
  + 修复 uni-id Apple 登录时用户邮箱为空时报错的Bug
  + 修复 uni-id 用户名密码登录时多个应用出现重复用户名登录报错的Bug
  + 修复 本地调试插件 打开非云函数根目录文件时使用运行菜单本地运行云函数报错的Bug
  + 修复 本地调试插件 部分情况下客户端连接启用了 JQL 扩展的本地云函数报错的Bug
* 【App插件(含5+App和uni-app的App端)】
  + 【重要】新增 Payment 模块支持 Paypal支付、Stripe支付、Google支付 [文档](https://uniapp.dcloud.io/app-payment)
  + 【重要】新增 Push 模块支持 Google推送 Firebase Cloud Push (FCM) [文档](https://uniapp.dcloud.io/app-push-fcm)
  + 【重要】新增 Statistic 模块支持 Google统计 [文档](https://uniapp.dcloud.io/app-statistic-google)
  + 新增 一键登录 支持 closeIcon 属性设置自定义关闭按钮图片 [文档](https://uniapp.dcloud.io/univerify)
  + 更新 uni-AD 快手广告SDK Android为 3.3.20 版，iOS为 3.3.20 版；快手内容联盟SDK Android为 3.3.27 版， iOS为 3.3.27 版
  + Android平台 修复 调用 plus.runtime.restart 重启应用后 user-agent 会清空的Bug [详情](https://ask.dcloud.net.cn/question/136105)
  + Android平台 修复 plus.downloader.enumerate 可能获取不到下载任务的Bug [详情](https://ask.dcloud.net.cn/question/137548)
  + Android平台 修复 一键登录 在部分 Android 8.0、8.1 设备无法弹出登录框的Bug
  + Android平台 修复 一键登录 设置登录界面 logo 图片可能不生效的Bug
  + Android平台 修复 视频播放控件 VideoPlayer 设置 object-fit 属性可能不生效的Bug [详情](https://ask.dcloud.net.cn/question/137150)
  + Android平台 修复 使用系统定位模块执行 watchPosition 后再执行 getCurrentPosition 可能失败的Bug [详情](https://ask.dcloud.net.cn/question/137586)
  + Android平台 修复 Push模块 createMessage 在安卓系统8以下系统可能无法创建通知栏消息的Bug [详情](https://ask.dcloud.net.cn/question/137923)
  + Android平台 修复 图片选择界面设置 crop 属性在部分手机和模拟器上可能引起黑屏崩溃的Bug [详情](https://ask.dcloud.net.cn/question/136969)
  + Android平台 修复 图片选择界面未勾选`原图`时图片方向可能发生变化的Bug [详情](https://ask.dcloud.net.cn/question/137358)
  + iOS平台 修复 uni-AD 使用自定义 storyboard 时开屏广告底部应用图标、名称可能不显示的Bug
* 【uni小程序SDK】
  + 新增 小程序 wgt 资源文件支持加密 [文档](https://nativesupport.dcloud.net.cn/UniMPDocs/API/ios?id=installWgt)
  + Android平台 修复 不设置任何参数初始化小程序SDK可能会引起崩溃的Bug [详情](https://ask.dcloud.net.cn/question/137175)
  + Android平台 修复 启动使用 vue3 的小程序可能出现白屏的Bug
  + iOS平台 修复 小程序未开启后台运行，通过手势关闭小程序后快速打开小程序偶现崩溃的Bug
  + iOS平台 修复 在隐藏小程序的回调方法中再次打开同一小程序无效的Bug
  + iOS平台 修复 同时打开多个小程序 getCurrentPageUrl 获取当前显示的小程序页面路径不正确的Bug

## 历史更新日志
[https://update.dcloud.net.cn/hbuilderx/changelog/ReleaseNote_alpha_archive.html](https://update.dcloud.net.cn/hbuilderx/changelog/ReleaseNote_alpha_archive.html)
