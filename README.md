# CardView
CardView层叠样式
今天主要是CardView的用法，CardView是在安卓5.0提出的卡片式控件。
首先在gradle文件下添加依赖库：
```
compile 'com.android.support:cardview-v7:22.2.1'
```
##### 它的基本属性如下： 
```
app:cardBackgroundColor这是设置背景颜色 
app:cardCornerRadius这是设置圆角大小 
app:cardElevation这是设置z轴的阴影 
app:cardMaxElevation这是设置z轴的最大高度值 
app:cardUseCompatPadding是否使用CompatPadding 
app:cardPreventCornerOverlap是否使用PreventCornerOverlap 
app:contentPadding 设置内容的padding 
app:contentPaddingLeft 设置内容的左padding 
app:contentPaddingTop 设置内容的上padding 
app:contentPaddingRight 设置内容的右padding 
app:contentPaddingBottom 设置内容的底padding
```
##### CardView是在布局中使用的：
```
<android.support.v7.widget.CardView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        app:cardBackgroundColor="#efefef"
        app:cardCornerRadius="15dp"
        app:cardElevation="80dp"
        app:cardPreventCornerOverlap="true"
        app:cardUseCompatPadding="true"
        app:contentPadding="20dp">
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="100dp"
            android:orientation="vertical">
            <ImageView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:src="@mipmap/ic_launcher"/>
            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:id="@+id/tView"/>
        </LinearLayout>
    </android.support.v7.widget.CardView>
```
