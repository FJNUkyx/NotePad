# 期中实验-NotePad笔记本应用

**效果介绍**

打开记事本app，点击右上角菜单

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020122023033290.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)


点击New note,编写第一个记事本，内容为This is first note,点击右上角菜单，点击Revert changes清空，点击delete删除当前记事本，点击Save保存

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220204112745.JPG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

分别新建了两个记事本，标题默认为记事本内容

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220204441862.JPG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

点进一个记事本，点击右上角菜单

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220204555565.JPG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

点击Editor title编辑标题

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220204756737.JPG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

编辑记事本标题为1

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220204902239.JPG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220205638969.JPG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/202012202052045.JPG)

点击右上角菜单的Search按钮进行记事本搜索

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220205316507.JPG)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220205330182.JPG)

修改记事本背景颜色，点进一个记事本，点击右上角菜单的Color

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220205443992.JPG)

选择一种颜色作为背景色

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220205516589.JPG)



### 一、基本要求：添加时间戳、根据标题查询
#### 1.添加时间戳
在noteslist_item.xml中添加显示时间戳的TextView

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220185248420.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

在NotePadProvider.java中添加创建时间、修改时间

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220185550941.png)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220185727337.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

在onCreate方法中添加创建时间、修改时间

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220185947232.png)

在NotesList.java中添加修改时间

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220190308462.png)

在dataColumns和viewIDs中添加修改时间

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220190500624.png)

在NotePadProvider.java中设置时间戳显示格式为yyyy.MM.dd HH:mm:ss

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220190848455.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

在NoteEditor.java中也要设置时间戳

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220191142730.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

运行结果截图：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220191303183.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

#### 2.实现根据标题查询
在list_options_menu.xml中加入搜索功能的item

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220191729808.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

在NotesList.java中的onOptionsItemSelected方法加入搜索功能的case语句

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220192006890.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

在layout里新建搜索功能的布局文件note_search_list.xml，代码如下：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220192211617.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

创建类NoteSearch.java,继承ListView,实现SearchView.OnQueryTextListener接口，加入创建时间

![](https://img-blog.csdnimg.cn/20201220193043297.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

为查询文本框注册监听器

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220193202728.png)

onQueryTextChange方法使用适配器SimpleCursorAdapter

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220193707867.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

最后再AndroidManifest.ml中注册搜索功能的类NoteSearch

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220194515114.png)

运行结果截图：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220194832103.png)

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020122019480345.png)
### 二、附加功能：修改背景颜色、日夜间模式
#### 1.修改背景颜色
在values中新建color.xml，定义背景的七种颜色

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220200042105.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

在layout中新建note_color.xml，在线性布局中创建七个颜色按钮

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220200425427.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220200459644.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020122020052815.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

新建NoteColor.java,代码如下：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220200929836.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220201059128.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220201130690.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220201159230.png)

在AndroidManifest.xml中注册背景颜色类NoteColor

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220201336783.png)

在NotePad.java中加入背景颜色字段

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220201549313.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

在NotePadProvider.java中的insert方法添加背景颜色的代码，默认颜色为白色

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220201827494.png)

新建一个MyCursorAdapter.java,继承SimpleCursorAdapter,用cursor读取数据库的内容，并填充颜色

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220202720993.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220202804683.png)

在editor_options_menu.xml中添加修改背景颜色

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220203050652.png)

在NoteEditor.java的onOptionsItemSelected方法中添加背景颜色的case

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220203342839.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

运行结果截图：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220203442211.JPG)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201220203512622.JPG)

#### 2.日夜间模式
在color.xml中定义两组颜色，分别表示日间和夜间的主题色

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201221010230538.png)

在styles.xml中定义两种主题，日间/夜间主题


```
<style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
      <item name="colorPrimary">@color/colorPrimary</item>
      <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
      <item name="colorAccent">@color/colorAccent</item>
      <item name="android:textColor">@android:color/black</item>
      <item name="mainBackground">@android:color/white</item>
     </style>
     
     <style name="NightAppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
      <item name="colorPrimary">@color/nightColorPrimary</item>
      <item name="colorPrimaryDark">@color/nightColorPrimaryDark</item>
      <item name="colorAccent">@color/nightColorAccent</item>
      <item name="android:textColor">@android:color/white</item>
      <item name="mainBackground">@color/nightColorPrimaryDark</item>
     </style>
```
新建一个mainBackground.xml,用来表示背景色
```
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <attr name="mainBackground" format="color|reference"></attr>
</resources>
```
在布局中加入切换按钮
```
<Button
  android:id="@+id/btn_theme"
  android:layout_width="match_parent"
  android:layout_height="wrap_content"
  android:text="切换日/夜间" />
  ```
 
判断是否有主题存储
 ```
 // 默认是日间模式
 private int theme = R.style.AppTheme;
 
 @Override
 protected void onCreate(Bundle savedInstanceState) {
  super.onCreate(savedInstanceState);
 // 判断是否有主题存储
  if(savedInstanceState != null){
   theme = savedInstanceState.getInt("theme");
   setTheme(theme);
  }
  Button btn_theme = (Button) findViewById(R.id.btn_theme);
  btn_theme.setOnClickListener(new View.OnClickListener() {
   @Override
   public void onClick(View v) {
    theme = (theme == R.style.AppTheme) ? R.style.NightAppTheme : R.style.AppTheme;
    MainActivity.this.recreate();
   }
  });
 }
 
 @Override
 protected void onSaveInstanceState(Bundle outState) {
  super.onSaveInstanceState(outState);
  outState.putInt("theme", theme);
 }
 
 @Override
 protected void onRestoreInstanceState(Bundle savedInstanceState) {
  super.onRestoreInstanceState(savedInstanceState);
  theme = savedInstanceState.getInt("theme");
 }

  ```
运行结果截图：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201221005617126.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020122100544022.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDcyODUzNw==,size_16,color_FFFFFF,t_70)
