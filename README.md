# Android-PhoneGap
在eclipse 中使用PhoneGap

## 将cordova的jar包添加到lib下

## 代码
在MainActivity中，把继承类由Activity改为DroidGap,将要显示的页面放在asset目录下,在onCreate方法中通过
super.loadUrl("file:///android_asset/www/index.html");加载进来


    public class MainActivity extends DroidGap {

    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        super.loadUrl("file:///android_asset/www/index.html");
    }

    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        getMenuInflater().inflate(R.menu.main, menu);
        return true;
    }   
    }

