##Android 面试目录  SageLu
[我的Github](https://github.com/SageLu "SageLu的gitub")

    	Activity 的生命周期是什么？ onPause 和 onStop 有什么区别？
		Android 五种布局的性能对比？
		Android 四大组件是什么？分别说说对它们的理解？
		关于 Service 的理解？它的启动方式有什么区别？
		了解 fragment 吗？说说你对它的理解？
		自定义过 view 吗？它的步骤是什么？说说你自定义 view 过程中出现的问题，以及是如何解决的？
		刷新 view 的几种方式，他们有什么区别？
		Android 实现数据存储的几种方式？
		如何实现 Android 中的缓存的，通过使用第三方库和自定义来分别说明一下缓存技术的实现？
		如何实现 Activity 与 fragment 的通信？
		Android 5.0、6.0、7.0 新特性？
		Android 中的动画分类？
		你以前是如何进行屏幕适配的？
		说说 Activity 创建过程？
		Android 中如何与 JS 交互的？
		了解 APP 的启动流程？
		你知道哪些图片加载库？他们有什么区别？ImageLoader 的内部缓存机制是什么？是如何实现的？
		Android 中是如何实现异步通信的？
		说说 Handler 内部实现原理？
		使用过 AsyncTask 吗？说说它的内部实现原理？它有什么缺陷？如何改进？
		知道 JNI、Binder 吗？说说你对它们的理解？
		如何实现进程间的通信？
		说说 Android view 和 viewGroup 的事件分发机制？
		你开发过程中使用到了哪些第三方库？了解过他们的源码吗？
		你了解广播吗？它与 EventBus 有什么区别？能互相实现吗？
		你们网络请求是如何实现的？知道 Volley 吗？内部实现流程是什么？它与 OKHttp 有什么区别？
		你了解哪些第三方功能？知道推送吗？它的原理是什么？
		接触过 MVP 模式吗？说说看对它的认识？
		知道 Android 中的多渠道打包吗？
		Android 签名机制的原理？反编译解压后的文件夹所包含的内容有哪些？
		你了解过模块化、组件化开发吗？
		开始开发 APP 如何进行架构？
		APP 工程模块是如何划分的？你是如何进行封装的？
		APP 是如何进行优化的？知道 OOM 吗？如何解决内存泄漏？
		手画一下Android系统架构图，描述一下各个层次的作用？
		Activity如与Service通信？
		Service的生命周期与启动方法由什么区别？
		Service先start再bind如何关闭service，为什么bindService可以跟Activity生命周期联动？
		广播分为哪几种，应用场景是什么？
		广播的两种注册方式有什么区别？
		广播发送和接收的原理了解吗？
		广播传输的数据是否有限制，是多少，为什么要限制？
		ContentProvider、ContentResolver与ContentObserver之间的关系是什么？
		遇到过哪些关于Fragment的问题，如何处理的？
		Android里的Intent传递的数据有大小限制吗，如何解决？
		描述一下Android的事件分发机制？
		描述一下View的绘制原理？
		requestLayout()、invalidate()与postInvalidate()有什么区别？
		Scroller用过吗，了解它的原理吗？
		了解APK的打包流程吗，描述一下？
		了解APK的打包流程吗，描述一下？
		了解APK的安装流程吗，描述一下？
		当点击一个应用图标以后，都发生了什么，描述一下这个过程？
		BroadcastReceiver与LocalBroadcastReceiver有什么区别？
		Android Handler机制是做什么的，原理了解吗？
		Android Binder机制是做什么的，为什么选用Binder，原理了解吗？
		描述一下Activity的生命周期，这些生命周期是如何管理的？
		Activity的通信方式有哪些？
		Android应用里有几种Context对象，
		描述一下进程和Application的生命周期？
		Android哪些情况会导致内存泄漏，如何分析内存泄漏？
		Android有哪几种进程，是如何管理的？
		SharePreference性能优化，可以做进程同步吗？
		如何做SQLite升级？
		进程保护如何做，如何唤醒其他进程？
		理解序列化吗，Android为什么引入Parcelable？
		如何计算一个Bitmap占用内存的大小，怎么保证加载Bitmap不产生内存溢出？
		Android如何在不压缩的情况下加载高清大图？
		Android里的内存缓存和磁盘缓存是怎么实现的。
		PathClassLoader与DexClassLoader有什么区别？
		WebView优化了解吗，如何提高WebView的加载速度？
		Java和JS的相互调用怎么实现，有做过什么优化吗？
		JNI了解吗，Java与C++如何相互调用？
		了解插件化和热修复吗，它们有什么区别，理解它们的原理吗？
		如何做性能优化？
		如果防止过度绘制，如何做布局优化？
		如何提交代码质量？
		有没有遇到64k问题，为什么，如何解决？
		MVC、MVP与MVVM之间的对比分析？
		如何导入外部数据库
		intentService作用是什么,AIDL解决了什么问题-小米
		Android属性动画特性-乐视-小米
		描述一次网络请求的流程-新浪
		Handler 消息处理
		LaunchMode应用场景-百度-小米-乐视
		Touch事件传递流程-小米
		View绘制流程-百度
		多线程-360
		线程同步-百度
		什么情况导致内存泄漏-美团
		垃圾回收
		ANR定位和修正
		什么情况导致oom-乐视-美团
		Service与Activity之间通信的几种方式
		如何保证service在后台不被Kill
		Requestlayout,onlayout,onDraw,DrawChild区别与联系-猎豹
		Android为每个应用程序分配的内存大小是多少-美团
		LinearLayout和RelativeLayout性能对比-百度
		优化自定义view百度-乐视-小米
		进程间通讯机制Binder
		Fragment生命周期
		volley解析-美团-乐视
		Glide源码解析
		Android设计模式
		架构设计-搜狐

