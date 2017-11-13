
![惯例先上图](https://gitee.com/ranchaoqun/ZTheme/blob/master/Screenrecorder-2017-11-13-14-58-58-832.gif "Demo效果图")
- ZTheme 使用示例
1.  创建ZTheme方法声明

```
    ZTheme createTheme(String apkPath, Context context);
    ZTheme createTheme(String apkPath, String libraryPath, Context context)

```
2. 使用apk创建ZTheme对象
```
     mZTheme = ZTheme.createTheme("/sdcard/theme/theme_dark.apk", this);

```
3.创建 ZThemeView  方法声明
```
    //根据反射创建ZThemeView对象，此处传入类名
    IThemeView getThemeView(String className)

```
4.创建 ZThemeView 对象
```
    IThemeView.getThemeView("com.rxx.ztheme.dark.view.LoginView");
```

5.最后就可以获取到一个view，加载到Activity。
```
  setContentView(IThemeView.getView());
```


