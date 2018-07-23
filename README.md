# xShadowLayout
Custom shading color library

## 阴影布局(继承FrameLayout) ##



[https://github.com/itfengan/xShadowLayout](https://github.com/itfengan/xShadowLayout)

效果图

![效果](http://img.blog.csdn.net/20171010160954830?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvZmVuZ2FuaXQ=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

布局文件

     	<?xml version="1.0" encoding="utf-8"?>
	<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/activity_main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="@dimen/activity_vertical_margin"
    android:paddingLeft="@dimen/activity_horizontal_margin"
    android:paddingRight="@dimen/activity_horizontal_margin"
    android:paddingTop="@dimen/activity_vertical_margin"
    tools:context="fengan.shadowdemo.MainActivity">
    <fengan.shadowdemo.ShadowLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:fengan_shadowed="true"
        app:fengan_shadow_angle="45"
        android:layout_centerInParent="true"
        app:fengan_shadow_radius="6dp"
        app:fengan_shadow_distance="10dp"
        app:fengan_shadow_color="#883F51B5">
        <TextView
            android:layout_width="250dp"
            android:layout_height="250dp"
            android:background="@drawable/bg"
            android:gravity="center"
            android:text="Hello World!"
            android:textColor="#ffffff"
            android:textSize="19sp"/>
    </fengan.shadowdemo.ShadowLayout>
	</RelativeLayout>



自定义属性attrs.xml

    <?xml version="1.0" encoding="utf-8"?>
	<resources>

    <declare-styleable name="ShadowLayout">
        <attr name="fengan_shadowed" format="boolean"/>
        <attr name="fengan_shadow_distance" format="dimension"/>
        <attr name="fengan_shadow_angle" format="integer"/>
        <attr name="fengan_shadow_radius" format="dimension"/>
        <attr name="fengan_shadow_color" format="color"/>
    </declare-styleable>

	</resources>
有灵性的小哥哥们，已经猜到这些属性对应的意思啦．．．
在此整理方便大家日后使用．．．
