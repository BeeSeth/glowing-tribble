# HBuilder X - Release Notes
======================================
## 3.7.0.20230118-alpha
### HBuilder
* Fixed the bug that HBuilderX cannot be started due to abnormal editor theme configuration in some cases.
* Fixed the bug that blank characters cannot be highlighted in the Markdown code area.
* Fixed the bug that Markdown copied table data from WPS and pasted it as a Markdown table syntax conversion error.
* Fixed the bug that the editor will not automatically scroll to the original cursor position when you press the esc key to find symbol in Editor.
* Language Server: Fixed the Vue file, when there are only script and style nodes, but no template node, the document structure diagram shows a blank bug.
* uniCloud: Fixed the bug that the upload and run operation fails when there are Chinese files in the cloud function directory of uniCloud cloud function.
* Mobile App Playground: MacOSX run the project to the real iOS device, and automatically start the App (MacOSX needs to install Xcode that matches the iOS mobile phone system) [Details](https://uniapp.dcloud.net.cn/tutorial/run/run-app.html#ios-app-automatically-open)
* Mobile App Playground: Added Windows operating system, iOS standard base, supports signing with Apple certificate, after signing, it can run standard base to iOS real device [Details](https://uniapp.dcloud.net.cn/tutorial/run/ios-apple-certificate-signature.html)
* Mobile App Playground: Added Windows device selection window, custom dock and standard dock support switching with & shortcut keys.
* uni-app: Added WeChat Build, automatically uploaded to the WeChat platform, and supports the configuration of WeChat ci robot numbers. [Details](https://uniapp.dcloud.net.cn/tutorial/build/publish-mp-weixin-cli.html)
* uni-app: uts plug-in run to Android support debug debugging [Details](https://uniapp.dcloud.net.cn/tutorial/debug/uni-uts-debug.html)
### uni-app plugin
* [Important] Added uts components. Native extensions can be developed using the uts language [Details](https://uniapp.dcloud.net.cn/plugin/uts-component.html)
* Added uni-vue-devtools plugin. Easy to view, modify data and review custom components [Details](https://uniapp.dcloud.net.cn/tutorial/debug/uni-vue-devtools.html)
* Web, App Added The page-meta component supports the scroll-top property
* Web Fixed The Vue3 project scroll-view component slot introduced in version 3.6.16 renders abnormally in some cases [Details](https://ask.dcloud.net.cn/question/149557)
* Web Fixed The show-progress attribute of the video component does not take effect [Details](https://github.com/dcloudio/uni-app/issues/3908)
* Web Fixed When the input component type=digit, the placeholder is not displayed after clearing the input box [Details](https://ask.dcloud.net.cn/question/160726)
* Web Fixed Vue3 project onNavigationBarSearchInputConfirmed not working [Details](https://ask.dcloud.net.cn/question/154740)
* Web Fixed Vue3 project switching tabbar page does not trigger onTabItemTap
* App Added [ext component] animation-view component [Details](https://uniapp.dcloud.net.cn/component/animation-view.html)
* App Fixed When the native navigation bar type in the Vue3 project is transparent, the color of the custom buttons does not change when sliding to the top on the navigation bar [Details](https://ask.dcloud.net.cn/question/154074)
* Weixin Mini Program Added pages.json supports configuring the entryPagePath property [Details](https://ask.dcloud.net.cn/question/126216)
* Weixin Mini Program Fixed An error is reported when running the enterprise version of WeChat introduced by version 3.6.16
* Weixin Mini Program Fixed Version 3.6.16 introduced Vue2 project partially in the scope slot access length property reported an error
* Weixin Mini Program Fixed Incorrect return value when using uni.env in Vue2 project [Details](https://ask.dcloud.net.cn/question/159865)
* Alipay Mini Program Fixed The DingTalk mini program uses uni.saveImageToPhotosAlbum to report an error [Details](https://ask.dcloud.net.cn/question/159183)
* Alipay Mini Program Fixed The platform property returned by uni.getSystemInfo was incorrect in the simulator
* QQ Mini Program Fixed The ended event of the video component of the Vue3 project does not trigger on the real machine [Details](https://ask.dcloud.net.cn/question/155602)
### uniCloud plugin
* Added Manage dependencies of schema extension [Details](https://uniapp.dcloud.net.cn/uniCloud/jql.html#deps-of-jql)
* Added JQL Trigger method add new parameters [Details](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#trigger-param)
### App plugin (5+ App & uni-app)
* Android Fixed The system navigation bar button color is the same as the background color caused by version 3.6.17 [Details](https://ask.dcloud.net.cn/question/161501)
* Android Fixed Picture selection on Android 13 devices prompts no permission [Details](https://ask.dcloud.net.cn/question/160879)
* Android Fixed plus.io.FileReader's readAsDataURL reads data without splitting by slice position [Details](https://ask.dcloud.net.cn/question/160467)
* Android Fixed The VideoPlayer fires the timeupdate event when the video is buffered

## 3.6.17.20230111-alpha
### uni-app plugin
* App Fixed 3.6.16 The Vue3 project in the vue page in the inner style of the rpx rendering error [Details](https://ask.dcloud.net.cn/question/161256)
* Weixin Mini Program Fixed 3.6.16 The VUE2 project part of the template uses multiple logical expressions in the template to run an error [Details](https://ask.dcloud.net.cn/question/161190)
### App plugin (5+ App & uni-app)
* Android Fixed After using the record module, the wgt upgrade prompt that the record module is not configured caused by version 3.6.11 [Details](https://ask.dcloud.net.cn/question/161167)
* Android Fixed The immersive status bar fails on some devices caused by version 3.6.16 [Details](https://ask.dcloud.net.cn/question/161277)

## 3.6.16.20230109-alpha
### HBuilder
* Language Server: Fixed the bug that the uni-app Vue file cannot be prompted for conditional compilation in the script tag [Details](https://ask.dcloud.net.cn/question/159783)
* Fixed HBuilderX green soft theme, select the terminal text, the bug that the selected color is not displayed.
* Optimize one-click sharing of Markdown, css and js resources required by the webpage, and upload them to uniCloud web page hosting.
* Fixed the bug that uni-app Vue3 runs to the browser, the browser Devtools console, and the log path shows errors.
* Fixed the bug that the uni-app runs to the iOS simulator, and the uni debugging is turned on. After opening, the window shows a blank bug
* Fixed the bug that in some cases, the .hbuilderx/launch.json file in the project root directory repeatedly writes data and reads and writes frequently, causing the editor to freeze
### uni-app plugin
* App-Vue, Web Updated The input component supports the inputmode property [Details](https://uniapp.dcloud.net.cn/component/input.html#inputmode)
* App Fixed The Vue3 project nvue page webview component onPostMessage event is invalid [Details](https://ask.dcloud.net.cn/question/158925)
* App Fixed The Vue3 project image component uses base64 to display exceptions [Details](https://ask.dcloud.net.cn/question/158368)
* App-Android Fixed The live-pusher component of the nvue page refuses the camera permission and then manually opens it. After returning to the application, the camera preview may not be called [Details](https://ask.dcloud.net.cn/question/158518)
* App-iOS Fixed The ad-content-page component of the nvue page cannot be re-pulled after failing to pull the advertisement configuration
* App-iOS Fixed After the nvue page map component uses a custom map style, switching satellite images is invalid [Details](https://ask.dcloud.net.cn/question/159316)
* App-iOS Fixed Start the application with a white screen after using the simulator to enable debugging [Details](https://ask.dcloud.net.cn/question/160363)
* Web Fixed, Mini Program Fixed Unstable Bug in uni-push2.0 [Details](https://ask.dcloud.net.cn/question/159690?item_id=224222&rf=false)
* Web Fixed The input component enters a negative number to bring out the last result [Details](https://ask.dcloud.net.cn/question/159447)
* Web Fixed Using uni.navigateTo eventChannel in Vue3 project will only be called once [Details](https://ask.dcloud.net.cn/question/155922)
* Web Fixed Vue3 project scroll-view component scrolling frequently triggers view updates [Details](https://ask.dcloud.net.cn/question/149557)
* Web Fixed The Vue3 project uses the picker component end attribute to read errors [Details](https://github.com/dcloudio/uni-app/issues/4075)
* Web Fixed uni.setTabBarItem causes tab switching life cycle exception [Details](https://ask.dcloud.net.cn/question/160739)
* Weixin Mini Program Fixed Array length changes cannot be observed in the Vue2 project template [Details](https://github.com/dcloudio/uni-app/issues/1827)
* Alipay Mini Program Fixed Vue3 project use inline styles running error report [Details](https://ask.dcloud.net.cn/question/159362)
### uniCloud plugin
* JQL Fixed Trigger report an error when using setUser without permission parameter
* JQL Fixed Add method report an error when using null in child object
* JQL Added Add triggerContext parameter to share variable between before trigger and after trigger [Details](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#trigger-context)
* Aliyun Updated Single file size limit was changed from 100MB to 5GB
### App plugin (5+ App & uni-app)
* Android Fixed Selecting files from system album may crash on some Harmony devices caused by version 3.6.12 [Details](https://ask.dcloud.net.cn/question/159556)
* Android Fixed Setting the targetSdkVersion value greater than or equal to 30 causes the app to crash when using AMap [Details](https://ask.dcloud.net.cn/question/159801)
* Android Fixed Multiple calls to createBLEConnection to connect to a Bluetooth device, failure to connect the device may also trigger a success callback [Details](https://ask.dcloud.net.cn/question/113070)
* iOS Fixed The iconWidth/iconHeight property is disabled when plus.nativeUI.toast sets style to inline [Details](https://ask.dcloud.net.cn/question/160192)
* iOS Fixed startBluetoothDevicesDiscovery Search for nearby Bluetooth devices returns data without an advertisData field [Details](https://ask.dcloud.net.cn/question/160178)

## 3.6.14.20221216-alpha
### HBuilder
* Fixed the bug caused by HBuilderX 3.6.12 that in some cases, the cursor position is wrong after the editor is pressed.
* Fixed the bug caused by HBuilderX 3.6.9 that in some cases, where the project root generated a 1.text test file.
* Fixed the bug that the html file exported by HBuilderX 3.6.7 runs to Chrome and starts a new Chrome instance.
* Fixed the bug that the uni-app web platform starts or stops browser Debugging, and in some cases, the console button is repeatedly displayed
### uni-app plugin
* App-Android Fixed After using the canvas module, the wgt upgrade prompt that the canvas module is not configured [Details](https://ask.dcloud.net.cn/question/159283)
* Mini Program Fixed Version 3.6.11 introduces an error after using async/await to run [Details](https://ask.dcloud.net.cn/question/159413)
### uniCloud plugin
* JQL Added `userInfo` and `result` to trigger parameter [userInfo](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#user-info)、[result](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#result)
* JQL Added `isEqualToJql` method to compare jql command [Details](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#is-equal-to-jql)
* JQL Updated Ignore null value of complex type (file, array, object) field
* HBuilderX Plugin Fixed Local cloud function server failed to start in some old operating systems [Details](https://ask.dcloud.net.cn/question/159343)
* HBuilderX Plugin Fixed the bug caused by HBuilderX 3.6.12, the debugging and running of cloud functions, and the Bug that cannot be debugged by Debug breakpoint.
* HBuilderX Plugin Fixed Aliyun business version cloud storage file is not visible in uniCloud web which was upload by local cloud function [Details](https://ask.dcloud.net.cn/question/159109)

## 3.6.12.20221207-alpha
* Fixed the bug that the uts file cannot display the outline view
* Fixed uts file, the bug that the right-click menu rearranges the code format is invalid
* Mobile App Playground: Optimize the device selection window, standard base and custom base, display base information
* Mobile App Playground: Optimize the menu [Run - Mobile App Playground], remove the menu [Select Playground]
* [uniCloud plugin]
  + HBuilderX Plugin Fixed The called function return noting causes error when call function by function

## 3.6.11.20221205-alpha
* Mobile App Playground: Added uts plug-in for running iOS standard base to iOS device
* Mobile App Playground: Added support for UDID display and replication in the iOS device selection window
* Mobile App Playground: iOS standard base installation package size, only supports arm64 architecture
* Mobile App Playground: Fixed the bug that the device selection window refreshes the device list and the radio at the bottom is changed
* Mobile App Playground: Fixed the bug that the Node process does not end in some cases when compiling and running the uts plugin
* uts plug-in: Added uts file Added conditional compilation, using //#ifdef APP-ANDROID and //#ifdef APP-IOS for platform conditional compilation
* uts plug-in: support for creating uts files and platform directories
* uts plug-in: Language service, improve code prompt speed, reduce memory usage
* uts plug-in: Compile cache is supported, no modification will not compile
* uts plug-in: Fixed language service, iOS platform, parameter tag name is the wrong keyword times Bug
* Language Server: Fixed the bug that the uni-app pages.json usingComponents code hints the typo [Details](https://ask.dcloud.net.cn/question/158601)
* HBuilderX: Fixed the bug that some plug-in functions will fail when closing the new HBuilder window or dragging the tab to create a new window.
* uniCloud: Fixed db_init.json to initialize the cloud database. When there are too many database tables, the bug of initializing the cloud database timeout.
* uniCloud: Added App packaging, console download link, one-click upload uniCloud, support to upload ipa or apk files to Aliyun official cloud storage.
* Fixed uni_modules plugin publish failed without category
* [uni-app plugin]
  + App Updated uts plugin supports compile cache
  + App Updated Vue2 project component.is support ComponentDefinition / ComponentConstructor [Details](https://ask.dcloud.net.cn/question/140044)
  + App Fixed The position calculation of nvue page slider component is inaccurate in some cases [Details](https://ask.dcloud.net.cn/question/152714)
  + Web Fixed The Vue3 project canvas component listens to the event and reports an error [Details](https://ask.dcloud.net.cn/question/158252)
  + Mini Program Updated The vue3 project uses import to import resources in non-static directories. After generation, the name is added to the hash by default. [Details](https://github.com/dcloudio/uni-app/issues/4011)
  + Weixin Mini Program Fixed Vue3 project v-for loop events may be messed up [Details](https://github.com/dcloudio/uni-app/issues/4015)
  + Weixin Mini Program Fixed Vue3 project wxs hot update fails [Details](https://ask.dcloud.net.cn/question/158252)
  + uni-im Full support for Vue3 [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-im.html)
* [uniCloud plugin]
  + JQL Added Trigger is supported, which can be used to excute some logic before or after database operation. Using jql syntax in trigger is supported. [Details](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#trigger)
  + JQL Fixed Using negative value as literal in where or permission cause error [Details](https://ask.dcloud.net.cn/question/157993)
  + JQL Added Using jql syntax in schema.ext is supported [Details](https://uniapp.dcloud.net.cn/uniCloud/jql-schema-ext.html#using-jql-syntax)
  + HBuilderX Plugin Fixed Action not found when call local clientDB or jql extension [Details](https://ask.dcloud.net.cn/question/157997)
  + uniIdRouter Fixed Router api error in vue3 project [Details](https://ask.dcloud.net.cn/question/158015)
  + uni-id-co Added password setting API [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#set-pwd)
  + uni-id-co Added external system joint login API, which can create an account corresponding to uni-id for the external system, so that the account can use the system and functions that depend on uniId [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#external)
  + uni-id-co Added authentication signature verification when HTTP requests [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#http-reqeust-auth)
  + uni-id-co Added error code `uni-id-account-not-exists-in-current-app` when the matched user cannot login in the current app  [Error Code Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#errcode)
  + uni-id-co Fixed error that the user did not set the avatar when logging in on WeChat
  + uni-id-co Fixed Unable to get uniIdToken from clientInfo
  + uni-id-pages Added Jump to set password page configuration item `setPasswordAfterLogin` after login [详情](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#set-pwd-after-login)
  + uni-id-pages Added setting password page
  + uni-id-pages Optimize toast error prompt time to 3 seconds
  + uni-admin Optimize schema file naming convention of the bulk SMS function, change `batch-sms-template` `batch-sms-task` `batch-sms-result` to `opendb-sms-temlate` `opendb-sms-task` `opendb-sms-log` conforms to the opendb specification.
* [App plugin (5+ App & uni-app)]
  + Added Record, Camera, Barcode, Orientation modules [Details](https://uniapp.dcloud.net.cn/tutorial/app-modules.html#bcor)
  + iOS Fixed Third-party login authorization does not trigger callback caused by version 3.6.10 [Details](https://ask.dcloud.net.cn/question/158380)

## 3.6.10.20221121-alpha
* Fixed the bug that HBuilderX 3.6.9 cannot compile and run normally when the uni-app CLI project has uts plug-in
* Fixed the uni-app uts plugin language service `import x from '@/uni_modules/'` uts plugin path error bug
* Mobile App Playground: Fixed the bug that HBuilderX crashes when you click the Run button in some cases in the device selection window
* Optimize uts plug-in iOS platform local compilation and real machine running speed
* [uni-app plugin]
  + App Fixed Vue2 project editing uts plugin code hot update invalid
  + uni-im supports projects that are not uniCloud or based on uni-id-pages [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-im.html)
  + App Fixed Vue2 project nvue page does not support the uts plugin [Details](https://ask.dcloud.net.cn/question/157435)
  + App Fixed Setting the statusBar color in darkmode is not normal
  + App Fixed nvue homepage setting navigationBarTextStyle is invalid [Details](https://ask.dcloud.net.cn/question/150485)
  + App Fixed that there is no text prompt for loading when uni.startSoterAuthentication (biometric identification) is wrong [Details](https://ask.dcloud.net.cn/question/157353)
  + App-Android Fixed uni.request does not support head requests [Details](https://ask.dcloud.net.cn/question/136717)
  + App-Android Fixed Getting focus cursor position may be incorrect when there are multiple input components in the page
  + App-Android Fiexed The nvue live-pusher component cannot be previewed on Android11+ devices using mobile networks [Details](https://ask.dcloud.net.cn/question/156532)
  + Web Fixed Vue3 project --window-top calculation error [Details](https://ask.dcloud.net.cn/question/157164)
  + Web Fixed Vue3 project configuration global loading and error components are invalid [Details](https://ask.dcloud.net.cn/question/157122)
  + Alipay Mini Program Fixed page-meta component root-font-size property invalid [Details](https://ask.dcloud.net.cn/question/157168)
* [uniCloud plugin]
  + [Important] Aliyun business version is avaliable [Details](https://ask.dcloud.net.cn/article/40144)
  + JQL Added "geoNear" stage is supported [Details](https://uniapp.dcloud.net.cn/uniCloud/jql.html#geo-near)
  + JQL Fixed Some legal jql requests falsely report permission errors
* [App plugin (5+ App & uni-app)]
  + Android Fixed Listen for the system dark mode theme switching event may be invalid [Details](https://ask.dcloud.net.cn/question/157497)
  + Android Fixed Cloud package using your owned certificates may report an 'Invalid keystore format' error [Details](https://ask.dcloud.net.cn/question/157057)
  + Android Fixed Cloud package fails when the package property value of AndroidManifest.xml is the same as the package name
  + iOS Fixed plus.screen.lockOrientation/plus.screen.unlockOrientation invalid on iOS16 devices [Details](https://ask.dcloud.net.cn/question/155357)
  + iOS Fixed Recording does not work when playing audio [Details](https://ask.dcloud.net.cn/question/157408)
  + iOS Fixed Setting DarkMode to follow the system theme may not work

## 3.6.9.20221114-alpha
* Added MarkDown, support for Mermaid diagrams, such as flow charts [Details](https://hx.dcloud.net.cn/Tutorial/Language/markdown?id=mermaid)
* Added MarkDown, code area, kotlin and uts with code highlighting support
* Added MarkDown, `! []()` and `[]()` syntax, support prompt file path [Details](https://hx.dcloud.net.cn/Tutorial/Language/markdown?id=PathHints)
* Language Server: Fixed a Bug where the image path prompt failed when an unsupported image format existed
* Language Server: Fixed a Bug where space was added to the first line of formatted ts files for MacOSX
* uts plug-in: Added iOS platform to support local compilation and real machine operation, need to configure Xcode environment. [Details](https://uniapp.dcloud.net.cn/tutorial/run/uts-development-ios.html)
* uts plug-in: Added Android platform, real machine operation supports three-party Gradle repository. [Details](https://uniapp.dcloud.net.cn/tutorial/run/uts-development-android.html)
* uts plug-in: Support code hints for iOS system API and Android system API.
* uts plug-in: Android platform Improve code hints for R resources.
* uts plug-in: Android platform supports import-free use of classes under java.lang.*
* HBuilderX: Fixed a Bug where the language service process would not exit when HBuilderX exits abnormally
* HBuilderX: Fixed a Bug that caused the built-in browser border to blink after dragging on some models of windows computers
* Mobile App Playground: iOS standard base, support the use of Apple certificate signature, after signature can run the standard base to iOS real device [Details](https://uniapp.dcloud.net.cn/tutorial/run/ios-apple-certificate-signature.html)
* Mobile App Playground: Fixed a Bug in the device selection window where HBuilderX was unable to perform any operations due to the error pop-up behind the device selection window in some cases
* Mobile App Playground: Fixed a Bug where the iOS offline SDK failed to synchronize files when the target was not HBuilder
* [uni-app plugin]
  + App, Web Add Support DarkMode [Details](https://uniapp.dcloud.net.cn/tutorial/darkmode.html)
  + App, Web Fixed Radio component disabled state style exception
  + App Add nvue page MapContext supports setLocMarkerIcon method  [Details](https://uniapp.dcloud.net.cn/api/location/map.html#setLocMarkerIcon)
  + App Fixed When Vue2 project uses composite API, onReady declaration cycle template ref is not bound
  + App Fixed Vue3 project template ref will be proxied
  + App Fixed Vue3 project setting the background color of the navigation bar to rgba is invalid [Details](https://ask.dcloud.net.cn/question/135111)
  + App Fixed Vue3 project root node height: 100% is invalid [Details](https://ask.dcloud.net.cn/question/156564)
  + App-iOS Fixed Vue3 project recording playback is invalid [Details](https://ask.dcloud.net.cn/question/155741)
  + Weixin Mini Program Fixed The Vue3 project defines global constants for compilation injection in vite.config.js, resulting in errors for clients using uniCloud introduced by version 3.6.8
  + Alipay Mini Program Fixed uni.showLoading prompts that the mask parameter is invalid [Details](https://ask.dcloud.net.cn/question/156944)
  + Alipay Mini Program Fixed Vue3 project eventChannel communication failed [Details](https://github.com/dcloudio/uni-app/issues/3945)
  + ByteDance Mini Program Updated component2 is enabled by default [Details](https://ask.dcloud.net.cn/question/156550)
* [uniCloud plugin]
  + [Important] Added uni-im cloud integrated, full platform, free, open source instant messaging system [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-im.html)
  + JQL Fixed Using add aggregate operator report an error [Details](https://ask.dcloud.net.cn/question/156261)
  + JQL Fixed Using some reserved js keywords in where or field report an error
  + JQL Fixed When querying a joined table with getTemp, an error bug is reported if the associated field of the main table is of array type in the schema but the actual data does not have this field
  + Cloud Object Added Call cloud object with url support mulit segment path [Details](https://uniapp.dcloud.net.cn/uniCloud/http.html#request-co-url)
  + HBuilderX Plugin Fixed The breakpoint entered the nodejs built-in module introduced by version 3.6.7
  + Secure Network Upgrade Uniform error code specification [Details](https://uniapp.dcloud.net.cn/uniCloud/secure-network.html#err-code)
  + uni-id-co Upgrade Using hmac-sha256 as password hash method [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#password-safe)
  + uni-id-co Added Support custom password hash/encrypt method [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#custom-password-encrypt)
  + uni-id-co Added Invoke uni-id-co using HTTP request [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#adapter-http)
* [App plugin (5+ App & uni-app)]
  + Added Stripe supports setting up billing information [Details](https://uniapp.dcloud.net.cn/tutorial/app-payment-stripe.html)
  + iOS Fixed TitleNView setting the default navigation bar color can cause inconsistencies with the status bar color
  + iOS Fixed setUIStyle setting dark mode may not work

## 3.6.8.20221027-alpha
* Mobile App Playground: Fixed, console, click on Object type log, after the editor is opened, the file content is not formatted bug
* [uni-app plugin]
  + Added Vue2 project Support for the use of composite APIs [Details](https://uniapp.dcloud.net.cn/tutorial/vue-composition-api.html)
  + Fixed Some objects inaccessible after using TypeScript in the Vue3 project derived from version 3.6.7 [Details](https://github.com/dcloudio/uni-app/issues/3930)
  + App, Web Added Location updates event [Details](https://uniapp.dcloud.net.cn/api/location/location-change.html)
  + App Updated Vue3 project Set minUserAgentVersion to 49 [Details](https://uniapp.dcloud.net.cn/collocation/manifest.html#appwebview)
  + App Fixed The nvue page global style of the Vue3 project is invalid from version 3.6.7 [Details](https://ask.dcloud.net.cn/question/155639)
  + App Fixed Vue2 project Event exception caused by remove page root node [Details](https://ask.dcloud.net.cn/question/155057)
  + App Fixed Vue2 project Updating data when the list does not use index as the key results in an event exception [Details](https://ask.dcloud.net.cn/question/155238)
  + App-Android Fixed uni.getStorageSync may report a 'SyntaxError' error in some cases [Details](https://ask.dcloud.net.cn/question/154284)
  + App-iOS Fixed The nvue page occasionally crashes when turning off or on the pull-down refresh on iOS16 devices
  + Web Fixed Vue2 project Using the page selector in CSS media queries does not take effect
  + Weixin Mini Program Added uni-AD rewarded video add secured callback [Details](https://uniapp.dcloud.net.cn/component/ad-weixin.html)
  + Alipay Mini Program Added Supports monitoring keyboard height changes using uni.onKeyboardHeightChange [Details](https://uniapp.dcloud.net.cn/api/key.html#onkeyboardheightchange)
  + Alipay Mini Program Fixed Events in the Mini Program component are triggered earlier and cannot be listened to in the Vue component
* [uniCloud plugin]
  + Added Secure Network, Added client verification to check client authenticity [Details](https://uniapp.dcloud.net.cn/uniCloud/secure-network.html#verify-client)
  + Added HBuilderX Plugin, Add [OpenDB Check for Updates] to the right-click menu of schema file which starts with 'uni-'
  + Added `uni-clear-temp-data` expired data and temporary file cleaning plugin [Details](https://ext.dcloud.net.cn/plugin?id=9826)
  + Fixed HBuilderX Plugin, Local cloudfuntion calls the redis interface report an error when transferring large data [Details](https://ask.dcloud.net.cn/question/155804)
  + Fixed uniIdRouter, Fix bug with incorrect uniIdRedirectUrl parameter when jumping using relative paths [Details](https://ask.dcloud.net.cn/question/155904)
  + uni-id-co Upgrade password encryption algorithm, support hmac-sha256 encryption [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#password-safe)
  + uni-id-co Added Developers can customize password encryption rules [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#custom-password-encrypt)
  + uni-id-co Added support for migrating other system users to uni-id [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#move-users-to-uni-id)
  + uni-id-co Support http requests [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#adapter-http)
* [App plugin (5+ App & uni-app)]
  + Android Fixed chooseVideo Using the camera to capture video may fail on Android 10 and above devices [Details](https://ask.dcloud.net.cn/question/155877)
  + iOS Fixed When sharing to WeChat favorites, jump to the moments [Details](https://ask.dcloud.net.cn/question/155362)

## 3.6.7.20221018-alpha
* Upgrade HBuilderX built-in Node version to 16.17.0 and built-in npm version to 6.14.12
* Git plug-in: git pull operation, Git message status bar, added log view function
* HBuilderX Settings: Aggregate language service-related configurations into the Language Service Configuration configuration item
* Added Node debugging, which supports attaching breakpoint debugging to the already started node process
* HBuilderX: Windows, pop-up prompts when the Node process is intercepted by security software, causing Node plug-ins such as language services to fail to start
* Language Server: Fixed a bug where when there were multiple CSS classes, quickly typing a space and then pressing the left button, causing the code prompt to replace the wrong position after carriage return
* Language Server: When entering a code block quickly, in some cases, the information on the right side of the code prompt window displays the bug of the results returned by other language services
* Language Server: Fixed the bug that the CSS code prompt speed is too slow for large CSS files
* Language Server: Fixed the bug of false positives in syntax verification in some cases when tsconfig.json exists in the uni-app project
* Language Server: Fixed the bug that in some cases, the language service frequently reported errors and crashed, and the bug of frequent pop-up errors in the lower right corner of the HBuilderX window
* Language Server: Fixed the bug that uni-app App.vue style introduced multiple files, and the class transfer definition only took effect on the last file
* Built-in browser: Fix the bug that HBuilderX crashes when dragging the built-in browser on some Windows computers
* Mobile App Playground: Fixed uni-app runs to the iOS simulator, modifies the nvue file, and cannot synchronize the modified bug
* Mobile App Playground: Fixed 5+App runs to iOS, in some cases, the log does not print the bug
* Added uni-app run to H5, debug, support to choose to use Chrome Debug, use the built-in browser to debug (click the bug icon in the console to pop up a selection menu)
* Fixed uni-app run to the Built-In Browser, In some cases, the bug of inconsistent cookies
* Added uni-app manifest.json, App module configuration, added "Secure Network"
* Fixed uniCloud Web Page Hosting, In some cases, the release fails and still performs the upload operation Bug
* Added uni_modules Supports configuration of module initialization scripts [Details](https://uniapp.dcloud.net.cn/plugin/uni_modules.html#package-json)
* [uni-app plugin]
  + [Important] Added uts iOS plugin [Details](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html)
  + [Important] Added `uni ext api`. Dipped the unusual API to the uni_modules plugin, but still use the uni. [Details](https://uniapp.dcloud.net.cn/api/extapi.html)
  + [Important] App-Android Fix the bug that the deviceId property of getSystemInfo occasionally fails to obtain and multiple devices are repeatedly obtained (note the backward compatibility problem caused by this modification) [Details](https://uniapp.dcloud.net.cn/api/system/info.html)
  + Vue3 project vite dependencies upgrade to the latest 3.1.8
  + App, Web Added Support uni.getBatteryInfo [Details](https://uniapp.dcloud.net.cn/api/system/batteryInfo.html)
  + App, Web Fixed Picker component date type cannot be used by the default year range [Details](https://ask.dcloud.net.cn/question/131332)
  + App, Web Fixed that the decimal point cannot be input on the numeric keyboard in iOS 16 [Details](https://ask.dcloud.net.cn/question/154584)
  + App, Web Fixed Editor component insertImage triggers input event does not have alt attributes [Details](https://ask.dcloud.net.cn/question/155163)
  + App, Web Fixed Vue3 project Editor component reloaded can not get EditorContext [Details](https://ask.dcloud.net.cn/question/154702)
  + App Added nvue page picker-view component adds mask-top-style, mask-bottom-style attributes [Details](https://uniapp.dcloud.net.cn/component/picker-view.html)
  + App Updated Video component supports the title attribute [Details](https://uniapp.dcloud.net.cn/component/video.html)
  + App Fixed hover-class attribute does not support multiple class [Details](https://ask.dcloud.net.cn/question/152506)
  + App Fixed Vue3 project ust plug-in export default class does not take effect [Details](https://ask.dcloud.net.cn/question/154164)
  + App Fixed Vue3 project v-for may rendering failure [Details](https://ask.dcloud.net.cn/question/154836)
  + App Fixed Vue3 project tabbar.broderStyle custom color value invalid [Details](https://ask.dcloud.net.cn/question/150718)
  + App Fixed Vue3 project nvue page switch component disabled attribute is invalid [Details](https://ask.dcloud.net.cn/question/154577)
  + App-Android Fixed in version 3.5.5 that caused the input component to automatically get the focus may fail [Details](https://ask.dcloud.net.cn/question/153481)
  + App-iOS Fixed nvue swiper component uses rpx may not slide properly to switch on some devices [Details](https://ask.dcloud.net.cn/question/149260)
  + Web Updated uni.preViewImage adds switching and closing buttons on the PC
  + Web Fixed Tabbar shows the duplicate Badge in some cases [Details](https://ask.dcloud.net.cn/question/153336)
  + Web Fixed uni.openLocation navigation does not automatically obtain the current position [Details](https://ask.dcloud.net.cn/question/155066)
  + Web Fixed Vue3 project titlenView's selection is not displayed when select is true [Details](https://ask.dcloud.net.cn/question/153179)
  + Web Fixed Vue3 project enters tabbar repeatedly trigger onLoad event [Details](https://ask.dcloud.net.cn/question/154066)
  + Web Fixed v-bind in the Vue3 project CSS does not take effect with rpx [Details](https://github.com/dcloudio/uni-app/issues/3884)
  + Mini Program Fixed When changing the data, setdata calls abnormalities [Details](https://github.com/dcloudio/uni-app/issues/3787)
  + Mini Program Fixed v-bind in the Vue3 project CSS does not take effect in the data in non-setup [Details](https://github.com/dcloudio/uni-app/issues/3887)
  + Mini Program Fixed Vue3 project action domain slot nesting may render failed when used [Details](https://github.com/dcloudio/uni-app/issues/3886)
  + Mini Program Fixed Vue3 project the static data rendering of the scoped slot is failed [Details](https://ask.dcloud.net.cn/question/153150)
  + Mini Program Fixed Vue3 project static data rendering errors in the role of the field slot [Details](https://ask.dcloud.net.cn/question/155008)
  + Mini Program Fixed The Vue3 project is issued to a mixed subcontract, and the page return may be reported to an error [Details](https://github.com/dcloudio/uni-app/issues/3923)
  + Weixin Mini Program Fixed drag-related events of the Vue3 project in scroll-view do not trigger [Details](https://github.com/dcloudio/uni-app/issues/3921)
  + Weixin Mini Program Fixed uni://form-field invalid in Vue3 project [Details](https://ask.dcloud.net.cn/question/155373)
  + Baidu Mini Program Fixed uni.createIntersectionObServer cannot listen to multiple nodes [Details](https://github.com/dcloudio/uni-app/issues/3835)
  + Baidu Mini Program Fixed Static resources in node_modules directory build error [Details](https://ask.dcloud.net.cn/question/154595)
  + Baidu Mini Program Fixed OnInit lifetimes is not triggered [Details](https://ask.dcloud.net.cn/question/154352)
  + Baidu Mini Program Fixed The Vue2 project uses usingSwanComponents to configure the event in the dynamic library component that cannot get parameters [Details](https://ask.dcloud.net.cn/question/155281)
  + Baidu Mini Program Fixed Vue3 project cannot use dynamic library components normally [Details](https://github.com/dcloudio/uni-app/issues/3864)
  + Alipay Mini Program Fixed After compiled into a mini program plug-in, uni.hideloading and other interfaces cannot be accessed [Details](https://github.com/dcloudio/uni-app/issues/2974)
  + Alipay Mini Program Fixed page-container component is compiled as a custom component [Details](https://ask.dcloud.net.cn/question/154028)
  + Alipay Mini Program Fixed invalid duration attribute in uni.showToast [Details](https://ask.dcloud.net.cn/question/147279)
  + Alipay Mini Program Fixed The component without events in the plug-in report an error [Details](https://github.com/dcloudio/uni-app/pull/3903)
  + QQ Mini Program Fixed Vue3 uni.createCanvasContext passing this returns an error [Details](https://ask.dcloud.net.cn/question/154223)
  + ByteDance Mini Program Added Support the use of mini program plugins [Details](https://github.com/dcloudio/uni-app/issues/3917)
  + ByteDance Mini Program Fixed Vue3 project uses mini program custom components that may report an error [Details](https://github.com/dcloudio/uni-app/issues/3915)
  + Kuaishou Mini Program Added Pages support subPackages [Details](https://uniapp.dcloud.net.cn/collocation/pages.html#subpackages)
  + Kuaishou Mini Program Update uni.requestPayment payment interface is compatible with calling ks.pay [Details](https://ask.dcloud.net.cn/question/152948)
  + uni-statistics Fixed The bug of inaccurate deviceId acquisition method caused by version 3.4.9, resulting in inaccurate statistics of unistatistics 2.0 App-Android platform [details](https://ask.dcloud.net.cn/article/40097)
* [uniCloud plugin]
  + Added Secure network, For secure communication between clients and cloud functions and cloud objects [Details](https://uniapp.dcloud.net.cn/uniCloud/secure-network.html)
  + Added uniCloud client sdk, Add uniCloud.databaseForJQL api to get database reference [Details](https://uniapp.dcloud.net.cn/uniCloud/clientdb.html#jssdk)
  + Added uniCloud client sdk, uniCloud.importObject add options.parseSystemError to parse uncaught exception for auto ui [Details](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#auto-ui)
  + Fixed UniCloud HBuilderX plugin, Require error is only reported once when connect to local cloud function
  + uni-id-co Added support for WeChat authorized mobile phone number login method [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#login-by-weixin-mobile)
  + uni-id-co Added Unbind third-party platform account [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#unbind-third-account)
  + uni-id-co Added WeChat binding mobile phone number to support `code` binding via `getPhoneNumber` event callback [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#bind-mobile-by-mp-weixin)
  + uni-admin Added bulk SMS function [Details](https://uniapp.dcloud.net.cn//uniCloud/admin.html#batch-sms)
  + uni-admin Fixed a bug where some statistics of the uni-statistics App-Android platform were inaccurate
  + uni-admin Fixed uni-statistics2 Bug where the week/month data is inaccurate
* [App plugin (5+ App & uni-app)]
  + Android Update the Paypal SDK to version 0.6.2, fixed the issue that setting targetSdkVersion to 31 packaging failed [Details](https://ask.dcloud.net.cn/question/154976)
  + Android Fixed plus.device.uuid may be getting same unique identity on different devices
  + Android Fixed App settings only support portrait when on some Android 8 devices may cause crash
  + Android Fixed LivePusher may cause the app to crash in some scenarios [Details](https://ask.dcloud.net.cn/question/147593)
  + Android Fixed The mute state of VideoPlayer may not work after switching video resources [Details](https://ask.dcloud.net.cn/question/153257)
  + Android Fixed VideoPlayer may cause stuttering when destroyed [Details](https://ask.dcloud.net.cn/question/153483)
  + Android Fixed VideoPlayer does not display the title bar in some cases
  + Android Fixed App does not work properly on Android 4.4 devices caused by version 3.6.2 [Details](https://ask.dcloud.net.cn/question/153910)
  + iOS Fixed VideoPlayer's title bar and progress bar style are incorrect [Details](https://ask.dcloud.net.cn/question/153945)
  + iOS Fixed Uni native language plugin Hook does not have applicationWillEnterForeground/applicationDidEnterBackground event caused by version 3.6.0

## 3.6.3.20220919-alpha
* Fixed the bug that the editor closes the tab, and crashes in some cases
* Fixed the bug of Windows built-in browser, mobile device mode, unable to select elements
* Fixed the bug that when switching to other programs during the HBuilderX code prompt process, the code prompt window would cover other programs in some cases
* Language Server: Fixed the bug of invalid px to rpx in uni-app cli project
* Fixed console log, some types of log output bugs
* Fixed the bug that uni-app runs to the iOS simulator, the console log is truncated or the output is incomplete
* Fixed the bug that uni-app runs to the Android emulator, and some Android emulators fail to run on Windows
* Fixed the bug that when uni-app runs to Android, in some cases, the console prompts that the compilation is successful, but there is no response
* Fixed the bug of App packaging failure caused by the new version of Alipay SDK for Android
* [uni-app plugin]
  + Mini Program Fixed onReady lifecycle fires twice [Details](https://ask.dcloud.net.cn/question/153422)

## 3.6.1.20220907-alpha
* Fixed the bug caused by HBuilderX 3.6.0, Windows, built-in browser, and network requests cannot be cross-domain
* Fixed the bug caused by HBuilderX 3.6.0, Windows, built-in browser, browser background color is wrong
* Fixed Editor, Close Tab, in some cases, the bug of not remembering the folded state
* Language Server: Fixed the bug of uni-app, pages.json, page field path prompting to complete the error after carriage return
* Language Server: Fixed uni-app, nvue file, css class, goto definition failed bug
* Language Server: Fixed the bug that uni-app, nvue files, script and style tags, could not prompt the lang attribute
* Language Server: Fixed JavaScript `Object.` does not prompt the bug of es6+ new methods
* Language Server: Fixed the bug that the stylus code in the Vue file has no prompts
* Language Server: Fixed `import xxx from 'XXX.vue'` without the vue suffix, prompting that the module cannot be found, and cannot go to the defined bug
* Language Server: Fixed the bug that the code prompt could not be automatically triggered when typing the character `.` in jsx and tsx files
* Language Server: Added built-in syntax check to support warning level
* Language Server: Fixed the bug that the `Script` node does not take effect in the Vue file when JavaScript verification is enabled
* Language Server: Fixed the bug that the error red wavy line still exists after the JavaScript verification function configuration is disabled in the html file
* Language Server: When there is a multi-line error, the mouse hovers over a non-first line, and the error message is not displayed.
* Mobile App - Cloud packaging: Fixed the bug that when the static resource file under the project is too large (over 100M), the packaged bug cannot be submitted
* Mobile App - Cloud packaging: Fixed the bug that HBuilderX crashed when submitting packaging in some cases on Windows
* [uni-app plugin]
  + App-Android Fixed uts plugin missing imported classes after compilation in some cases [Details](https://ask.dcloud.net.cn/question/152597)
  + App-Android Fixed When the uts plugin uses a kotlin basic type (such as Int) when defining a type, a compilation error is reported
  + App-Android Fixed uts plugin cloud package does not include AndroidManifest.xml
  + App-Android Fixed bindingx may cause exceptions when executing evaluatecolor [Details](https://ask.dcloud.net.cn/question/151759)
  + App-Android Fixed uni.reLaunch opens non-tabbar nvue pages may still show tabbar [Details](https://ask.dcloud.net.cn/question/143792)
  + App-Android Fixed AutoNavi Maps not working properly when setting GooglePlay channel [Details](https://ask.dcloud.net.cn/question/152668)
  + App-Android Fixed using the picker in nvue as homepage may cause the app to become unresponsive [Details](https://ask.dcloud.net.cn/question/151819)
  + App-iOS Fixed Nvue Tabbar page uni.reLaunch could not triggered onUnload lifetimes [Details](https://ask.dcloud.net.cn/question/152738)
  + Web Fixed Calling uni.setClipboardData will bring up the keyboard [Details](https://github.com/dcloudio/uni-app/issues/3569)
  + Mini Program Fixed Updated The Mini Program component supports the use of kebab-case event names [Details](https://github.com/dcloudio/uni-app/issues/1802)
  + Weixin Mini Program Fixed Calling triggerEvent in wxs cannot carry event parameters [Details](https://github.com/dcloudio/uni-app/issues/3829)
* [App plugin (5+ App & uni-app)]
  + Android Fixed Get the opposite width and height of a vertical video file with getVideoInfo [Details](https://ask.dcloud.net.cn/question/151205)
  + Android Fixed Offset may appear when previewing images with previewImage [Details](https://ask.dcloud.net.cn/question/151966)
  + iOS Fixed The uploadedSize value obtained by uploading a file using uploader is inaccurate

## 3.6.0.20220901-alpha
* Added UTS syntax support. Develop native using TypeScript [Details](https://en.uniapp.dcloud.io/tutorial/syntax-uts.html)
* Added the function of finding references, currently only supports js and ts
* Windows: Upgrade built-in browser, Upgrade Cef version to 90.6.7
* HBuilderX settings, plugin configuration, add configuration items, Enable JavaScript Validation, Enable TypeScript Validation
* Language Server: Added real-time verification of variable syntax in vue and js (js verification needs to be enabled in [Settings - Plugin Configuration])
* Language Server: Added vue3 `style module` to support code hints
* Language Server: Added vue2&3 `slot` to support code hints
* Language Server: Added vue2&3 script area to support automatic package import
* Language Server: Fixed the bug that vuedoc does not take effect in script setup
* Language Server: Fixed The custom component of vue3 `script setup` import, the bug that cannot be prompted in the template area
* Language Server: Fixed the bug that `()` will be repeatedly generated when modifying the name of the function call
* Language Server: Fixed the bug that special String does not support `if(idstr === '|')`
* Language Server: Fixed the bug that the variable suspension in the vue template area does not take effect
* Language Server: Fixed `uniCloud.importObject()`, after the cloud object is modified, the code prompt and suspension cannot take effect in real time
* Language Server: Optimized `uniCloud.importObject()`, code hints for parameters and return values ​​when calling methods on cloud objects
* Language Server: Fixed the bug that the framework package of the vetur specification could not take effect in real time when it was installed and uninstalled
* Language Server: Fixed the bug that the suspension of variables and functions referencing other files in the html script did not take effect
* Language Server: Fixed the bug that the return value and parameter type are incorrect when parsing the function that references other files in the html script
* Language Server: Fixed the bug that the frame syntax library of the status bar at the bottom of HBuilderX did not take effect when removed
* Language Server: Fixed the vue-cli project, the script area in vue will not recognize the bug of tsconfig.json under the project
* Language Server: Optimization After setting `px` to `rem`, the conversion prompt is placed in the first item of the code prompt
* Added tabs Right-click menu Add menus Move tabs to the left, move tabs to the right
* Windows: Fixed the bug that when HBuilderX is not started, when importing the plugin market plugin, the UI view of the first import shows a blank bug
* Fixed the bug that the jump position is wrong in some cases of multi-file character search
* Fixed the bug that when going back to another file, the cursor jumps to the beginning of the file instead of going to the position before the definition
* Added new project, HBuilderX plugin, added internationalization example template
* uni-app: Fixed manifest.json After the application name is internationalized, the packaging interface, the application name displays `%%`
* uni-app: Adjust the H5 configuration on the left side of manifest.json to the Web configuration
* [uni-app plugin]
  + [Important] Added uts Android plugin [Details](https://uniapp.dcloud.net.cn/plugin/uts-plugin.html)
  + App-iOS Fixed uni.openLocation bottom safe area adaptation problem [Details](https://ask.dcloud.net.cn/question/150074)
  + App-iOS Fixed That uni.chooseLocation may cause the app to crash [Details](https://ask.dcloud.net.cn/question/152367)
  + Web Added Support for configuring and using AutoNavi maps [Details](https://uniapp.dcloud.io/collocation/manifest?id=h5sdkconfigmaps)
  + Alipay Mini Program Fixed Compiling error after configuring global Mini Program components [Details](https://github.com/dcloudio/uni-app/issues/3619)
  + Alipay Mini Program Fixed Accessing $slots after enabling Mini Program Basic Library 2.0 configuration [Details](https://github.com/dcloudio/uni-app/issues/3529)
  + ByteDance Mini Program Added vue2 project to support onUploadDouyinVideo lifetimes [Details](https://ask.dcloud.net.cn/question/151113)
* [uniCloud plugin]
  + Updated UniCloud HBuilderX plugin, Change parameter of running cloud object by HBuilderX [Details](https://uniapp.dcloud.net.cn/uniCloud/rundebug.html#run-obj-param)
  + Fixed UniCloud HBuilderX plugin, Using push extension raise error which was triggered by HBuilderX 3.5.5
  + Fixed UniCloud HBuilderX plugin, Error "SIGN_PARAM_INVALID" occured occasionally which was triggered by HBuilderX 3.5.5
* [App plugin (5+ App & uni-app)]
  + iOS Fixed submit to App Store Connect report warning 'ITMS-90078: Missing Push Notification Entitlement' without push module

## 3.5.5.20220825-alpha
* Fixed the bug that the Windows HBuilderX Cli command is invalid
* Added Mobile App Playground, Device selection window, added base selection function
* Fixed Mobile App Playground, When the project path exists in Chinese and runs to an iOS device, the App page displays an abnormal bug
* Fixed Mobile App Playground, a bug where custom base installation failed in some cases
* Fixed uni-app manifest.json, a bug that the uniPush field becomes null in some cases
* [uni-app plugin]
  + Fixed Compile exception when project path contains parentheses. [Details](https://ask.dcloud.net.cn/question/150173)
  + App Fixed Vue page cover-view component flex layout is invalid. [Details](https://ask.dcloud.net.cn/question/151697)
  + App Fixed Vue3 project uni.getSystemInfo gets windowHeight value is inaccurate. [Details](https://ask.dcloud.net.cn/question/150862)
  + App Fixed Vue3 project vue page map component shows error after updating center coordinates. [Details](https://ask.dcloud.net.cn/question/151438)
  + App-Android Fixed uni.saveImageToPhotosAlbum saving network pictures may overwrite the last saved picture. [Details](https://ask.dcloud.net.cn/question/125357)
  + App-Android Fixed Picker component focus acquisition exception. [Details](https://ask.dcloud.net.cn/question/150454)
  + App-Android Fixed Nvue page map component customCallout setting image may cause application crash. [Details](https://ask.dcloud.net.cn/question/150166)
  + App-iOS Fixed The values of bluetoothEnabled and locationEnabled obtained by uni.getSystemSetting are inaccurate.
  + App-iOS Fixed The nvue page map component marker calls the moveAlong method without interrupting the previous animation. [Details](https://ask.dcloud.net.cn/question/151411)
  + App-iOS Fixed The nvue page ad-content-page component may cause the app to crash in some scenarios. [Details](https://ask.dcloud.net.cn/question/151778)
  + Web Fixed Vue3 project css environment variable --window-top calculation error. [Details](https://ask.dcloud.net.cn/question/150842)
  + Web Fixed Vue3 project release mode showLoading icon size display error. [Details](https://ask.dcloud.net.cn/question/149819)
  + Web Fixed custom-tab-bar component using uni.setTabBarItem to set visible is invalid. [Details](https://ask.dcloud.net.cn/question/132947)
  + Mini Program Fixed v-model fails after complex expressions are used in v-for. [Details](https://github.com/dcloudio/uni-app/issues/3173)
  + Alipay Mini Program, Baidu Mini Program, Kuaishou Mini Program, ByteDance Mini Program Updated Support automatic copying of ext.json files.
  + Alipay Mini Program Updated The uni.saveImageToPhotosAlbum interface no longer uses the legacy saveImage interface.
  + ByteDance Mini Program Fixed Component fails to render when repeatedly creating and destroying pages quickly.
* [uniCloud plugin]
  + Updated Aliyun Extend the timeout of database request from 3s to 5s
  + Added Aliyun Implement eip with http proxy provided by aliyun [Details](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#http-proxy-client)
  + Added CloudFunction Add context.requestId to get current request id in cloudfunction [Details](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#context)
  + Added CloudObject Add this.getUniCloudRequestId() to get current request id in cloudobject [Details](https://uniapp.dcloud.net.cn/uniCloud/cloud-obj.html#get-request-id)
  + Added CloudSdk Add uniCloud.getRequestList to get the list of request id being processed by current cloudfunction instance [Details](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#get-request-list)
  + Added CloudSdk Add uniCloud.getCloudInfos to get the list of cloud info being processed by current cloudfunction instance [Details](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#get-cloud-infos)
  + Added CloudSdk Add uniCloud.getClientInfos to get the list of client info being processed by current cloudfunction instance [Details](https://uniapp.dcloud.net.cn/uniCloud/cf-functions.html#get-cloud-infos)
  + Fixed ClientSdk Using uniCloud object cause error when uniCloud space was not bound to project [Details](https://github.com/dcloudio/uni-app/issues/3758)
  + Fixed JQL Multi parentKey in schema is unable to query with getTree [Details](https://ask.dcloud.net.cn/question/151834)
  + Fixed UniCloudDebugger Extension is not loaded properly in some situation [Details](https://ask.dcloud.net.cn/question/150357)
  + Fixed UniCloudDebugger Memory leak of dev server which cause slow responding
  + Updated uniIdRouter It's able to intercept home page or launch page loading now
  + Updated uni-id-co Password rule updated, password strength is configurable. [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#password-strength)
  + Updated uni-id-co Save user openid into `wx_openid.${mp|h5|app|web}` and `wx_openid.${mp|h5|app|web}_${DCloudAppId}` of user record [Login by weixin](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#login-by-weixin)、[Login by QQ](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#login-by-qq)
  + Updated uni-id-co Save user session_key, access_token with uni-open-bridge-common [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#save-user-token)
  + Added uni-id-co Add beforeRegister hook to manipulate user record before register [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-summary.html#before-register)
  + Added uni-id-pages Support login by weixin official account web page and wechat's qrcode of web page [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#weixinlogin)
  + Added uni-id-pages Support password strength (whether it must contain upper and lower case letters, numbers, special symbols and length) configuration [Details](https://uniapp.dcloud.net.cn/uniCloud/uni-id-pages.html#config)
  + Added uni-id-pages Add global login success event: `uni-id-pages-login-success`, listen this event by [uni.$on](https://uniapp.dcloud.net.cn/api/window/communication.html#on)
* [App plugin (5+ App & uni-app)]
  + Android Update the version of QQ login and sharing SDK to 3.5.12, the version of Baidu positioning SDK to 9.3.5, and the version of Baidu map SDK to 7.5.3
  + Android Fixed the payload field of vendor channel does not support non JSON strings in UniPush 2.0
  + Android Fixed the option parameter setting when field of creating local message with plus.push.createMessage is invalid
  + Android Fixed upgrade APK with plus.runtime.install may report null pointer
  + iOS Fixed use baidu location module needs enable IDFA caused by version 3.5.0
  + iOS Fixed the token value returned by univerify in the playground is incorrect caused by version 3.5.0
  + iOS Fixed the display time of slow motion video when select it from album is not accurate [Details](https://ask.dcloud.net.cn/question/150531)

## 3.5.4.20220805-alpha
* Fixed the bug that debug view, variable, Global node, UI display disorder
* Fixed the bug that HBuilderX saves files in utf-8 format without file header identification byte 0xEFBBBF
* [uni-app plugin]
  + App Updated The web-view for Vue2 project can use webviewStyles set more style. [Details](https://ask.dcloud.net.cn/question/149212)
  + App Updated The web-view for Vue page can drawn outside of safe area by default. [Details](https://ask.dcloud.net.cn/question/149472)
  + App-Android Fixed the bug that the overlapping coordinates of the nvue map marker points cannot be displayed [Details](https://ask.dcloud.net.cn/question/149665)
  + App-Android Fixed the bug that the nvue map component does not take effect when the polyline and polygon data are cleared
  + App-iOS Fixed the bug that uni.setTabBarItem dynamic update icon may not take effect [Details](https://ask.dcloud.net.cn/question/149955)
  + App-iOS Fixed the bug that the nvue map component may not be loaded properly in multiple pages when use Google map moudle [Details](https://ask.dcloud.net.cn/question/150080)
  + Web Updated The web-view component support props of fullscreen. [Details](https://uniapp.dcloud.net.cn/component/web-view.html)
  + Web Fixed The touch envet stop and prevent for canvas component are invalid. [Details](https://ask.dcloud.net.cn/question/148195)
  + Alipay Mini Program Fixed The project for Vue3 $slots is invalid. [Details](https://ask.dcloud.net.cn/question/150373)
* [uniCloud plugin]
  + Added IP anti-brushing for cloudfunction and clientDB [Details](https://uniapp.dcloud.net.cn/uniCloud/ip-filter.html)
  + Fixed use uniCloud inside main.js cause error in some situation
  + Fixed uni-admin vue3 The value of showLeftWindow is incorrect after uni.showLeftWindow was called [Details](https://ask.dcloud.net.cn/question/149618)
  + Added uni-statistics2 Add config item to set the duration of periodic reporting of data [Details](https://uniapp.dcloud.net.cn/uni-stat-v2.html#report-time)
* [App plugin (5+ App & uni-app)]
  + iOS Fixed the bug of cloud packaging error when use baidu map or geolocation modules without check `use IDFA` caused by version 3.5.0
  + iOS Fixed the bug of page fall back abnormally when app switches to the foreground and use splashscreen AD caused by version 3.5.3 [Details](https://ask.dcloud.net.cn/question/150053)
  + iOS Fixed the bug of chosse iCloud picture display black screen when setting the crop attribute [Details](https://ask.dcloud.net.cn/question/149219)

## 3.5.3.20220727-alpha
* Fixed the operating system environment variable, configuring `NODE_OPTIONS --openssl-legacy-provider`, HBuilderX loses response when it starts

## 3.5.2.20220719-alpha
* Git plugin, pull operation, the default option is changed to the fourth item, namely git pull --rebase --autostash
* Fixed the bug of plugin installation try move failed in some cases

## 3.5.1.20220707-alpha
* Added HBuilderX status bar Upgrade added red dot prompt
* Fixed the bug that the editor selects the language association window position offset
* Fixed the bug that the plugin API hx.window.showQuickPick() window could not scroll after opening the terminal
* Fixed some issues for language service

## 3.5.0.20220623-alpha
* Added TypeScript support for syntax verification
* Added MarkDown code block to support language coloring and highlighting, you need to download and add the corresponding language coloring extension plug-in
* Fixed language service React jsx file no code hint bug
* Fixed some minor issues

## 3.4.17.20220614-alpha
* Fixed the bug that plugin installation fails in some cases.
* Fixed the bug that the hover list disappears automatically when Windows opens the terminal, searches for categories in the toolbar, and moves the mouse to it.

## 3.4.13.20220601-alpha
* Added language service JavaScript supports DOM type recognition of id selectors in Document. getElementById and Document. querySelector
* Added language service SCSS support for prompt `!global` and `!default`
* Fixed some issues for language service

## 3.4.12.20220523-alpha
* Fixed a Bug where the left view project name does not show Git branch information

## 3.4.11.20220520-alpha
* HBuilderX improves startup speed
* Fixed some minor issues

## 3.4.10.20220517-alpha
* Added support for running and debugging Node programs
* Added syntax highlighting that can be independently extended for new languages, and language highlighting plug-ins can be developed or downloaded
* Some of the built-in language syntax highlighting was migrated to the plug-in marketplace
* Fixed multi-file search, the right side of the display code coloring error Bug
* Fixed plug-in installation window, installed plug-in, version number display error Bug
* Added language services, VUE-CLI projects, code hints support element-UI, bootstrap-vue, etc
* Fixed Emmet syntax bug where pressing TAB did not respond correctly
* Fixed language service, input CSS code in the same line, press Enter, replace the wrong position Bug
* Fixed language service,jsdoc carriage return error Bug

## 3.4.9.20220508-alpha
* Fixed some issues for language service

## 3.4.8.20220428-alpha
* Added HBuilderX Support for custom project Snippets
* Fixed some issues for language service

## 3.4.6.20220416-alpha
* Fixed some issues for language service
* Adjust Share to Weblink, adjust code area code coloring

## 3.4.5.20220408-alpha
* Fixed some issues for language service

## 3.4.4.20220403-alpha
* Fixed some issues for language service

## 3.4.3.20220325-alpha
* Fixed some minor issues

## 3.4.2.20220310-alpha
* Fixed some minor issues

## 3.4.1.20220308-alpha
* Fixed some minor issues

## 3.4.0.20220304-alpha
* HBuilderX language service switched from Java to Node
* Fixed a bug where files in the editor would not be automatically refreshed after Git updated files in some cases

## 3.3.12.20220222-alpha
* Fixed some minor issues

## 3.3.8.20220114-alpha
* Fixed some minor issues

## 3.3.7.20220112-alpha
* Fixed some minor issues

## 3.3.6.20211231-alpha
* Fixed some minor issues

## 3.3.2.20211218-alpha
* Fixed some minor issues

## 3.3.1.20211214-alpha
* Fixed a crash in the editor when Find Symbols by clicking on the search area or the built-in Explorer address bar.
* Fixed 3.3.0 for Windows HBuilderX maximization, editor window interface rendering exception.
* Fixed the Bug where MacOSX failed to run projects to iOS emulator when the HBuilderX installation path had a space.

## 3.3.0.20211130-alpha
* Adjust the UI of the new project window [Details](https://hx.dcloud.net.cn/Tutorial/project?id=CreateProjectWindows)
* Added project manager view toolbar, added positioning and folding functions [Details](https://hx.dcloud.net.cn/Tutorial/project?id=toolbar)

## 3.2.15.20211120-alpha
* Fixed some minor issues

## 3.2.14.20211112-alpha
* Fixed some minor issues

## 3.2.13.20211110-alpha
* Added Files larger than 1M in size do not display hover code assist
* Fixed the bug that caused the node process to fail to start when the max-old-space-size configured in the operating system environment variables was too large

## 3.2.12.20211028-alpha
* Fixed some minor issues

## 3.2.11.20211021-alpha
* Added HBuilderX plug-in development breakpoint debugging

## 3.2.10.20211013-alpha
* Added hover code assist [Details](https://hx.dcloud.net.cn/Tutorial/Language/Overview?id=hover-code-assist)
* Added Terminal supports clicking on the URL to jump to the browser [Details](https://hx.dcloud.net.cn/Tutorial/UserGuide/terminal?id=open-links)
* Fixed the bug that when the terminal input exceeds a certain length, the wrong line is displayed
* Fixed the bug that the editor window exceeds the screen area when creating multiple terminals
* Fixed the bug that the editor bookmarks are lost due to code formatting

## 3.2.8.20210923-alpha
* Fixed the bug that the EOL of the editor file is rendered incorrectly when the EOL is set to be displayed

## 3.2.7.20210919-alpha
* Added Configure whether you receive automatic updates.
* Fixed the bug that the editor crashes when a new project is created with / at the end of the storage path.
* Fixed Bug that HBuilderX editor cannot render Arabic
* Upgrade eslint-vue plugin.
* Fixed the bug of MacOSX system, open in terminal, the top content of the terminal is squeezed.
* The menu at the top of the HBuilderX editor [Help-License Agreement], adjusted to an online link, click to jump to the browser to open.

## 3.2.6.20210901-alpha
* Added HBuilderX supports localized language pack extension [Details](https://github.com/dcloudio/hbuilderx-language-packs)
* Vue3 improvements [Details](https://hx.dcloud.net.cn/Tutorial/Language/vue-next)
