## 本文主要是记录一下在日常开发中的一些总结和一些规范性的东西

###目录
* [android命名规范](#android命名规范)
* [android注意事项](#android注意事项)
* [android小技巧](#android小技巧)
* [android兼容性bug](#android兼容性bug)

##android命名规范
###1. id控件命名规范

<table>
    <thead>
	 <tr>
	  <td>控件名称</td>
	  <td>缩写</td>
	 </tr>
	</thead>
    <tbody>
	 <tr>
	  <td>LinearLayout</td>
	  <td>ll_</td>
	</tr>
 	 <tr>
	  <td>RelativeLayout</td>
	  <td>rl_</td>
	</tr>
    <tr>
	  <td>TextView</td>
	  <td>tv_</td>
	</tr>
	<tr>
	  <td>Button</td>
	  <td>btn_</td>
	</tr>
    <tr>
	  <td>ImageButton</td>
	  <td>ibtn_</td>
	</tr>
    <tr>
	  <td>ImageView</td>
	  <td>iv_</td>
	</tr>
	<tr>
	  <td>CheckBox</td>
	  <td>cb_</td>
	</tr>
    <tr>
	  <td>RadioButton</td>
	  <td>rbtn_</td>
	</tr>
	<tr>
	  <td>EditText</td>
	  <td>et_</td>
	</tr>
    <tr>
	  <td>ProgressBar</td>
	  <td>proBar_</td>
	</tr>
    <tr>
	  <td>SeekBar</td>
	  <td>skBar_</td>
	</tr>
	<tr>
	  <td>AutoCompleteTextView</td>
	  <td>autoTxt_</td>
	</tr>
	<tr>
	  <td>WebView</td>
	  <td>wbv_</td>
	</tr>
	<tr>
	  <td>RantingBar</td>
	  <td>ratBar_</td>
	</tr>
	<tr>
	  <td>Spinner</td>
	  <td>spn_</td>
	</tr>
	<tr>
	  <td>ScollView</td>
	  <td>slV_</td>
	</tr>
	<tr>
	  <td>TextSwitch</td>
	  <td>txtSwt_</td>
	</tr>
	<tr>
	  <td>ListView</td>
	  <td>lv_</td>
	</tr>
	<tr>
	  <td>ExpandableListView</td>
	  <td>epdLv_</td>
	</tr>
	<tr>
	  <td>DatePicker</td>
	  <td>dtPk_</td>
	</tr>
	<tr>
	  <td>TimePicker</td>
	  <td>tmPk_</td>
	</tr>
  </tbody>
</table>

###2. 资源文件命名规范
<table>
    <thead>
	 <tr>
	  <td>资源</td>
	  <td>命名规范</td>
	 </tr>
	</thead>
    <tbody>
	 <tr>
	  <td>colors.xml</td>
	  <td>项目简称_color_颜色英文_色值，比如：cs_color_yellow_ff484a</td>
	</tr>
 	 <tr>
	  <td>string.xml</td>
	  <td>项目简称_string_具体英文,比如：cs_string_cancle</td>
	</tr>
    <tr>
	  <td>styles.xml</td>
	  <td>针对TextView来说可以用 tv_颜色英文_色值_size字体大小,比如：tv_grey808080_size12</td>
	</tr>

  </tbody>
</table>

###3. 资源布局规范
<table>
    <thead>
	 <tr>
	  <td>Activity</td>
	  <td>activity_模块名称.xml,例如：activity_main.xml、activity_user.xml</td>
	 </tr>
	</thead>
    <tbody>
	 <tr>
	  <td>Fragment</td>
	  <td>fragment_模块名称.xml,例如：fragment_main.xml、fragment_user.xml</td>
	</tr>
 	 <tr>
	  <td>列表项</td>
	  <td>item_模块名称.xml</td>
	</tr>
    <tr>
	  <td>通用布局</td>
	  <td>common_布局的名称.xml，比如User的通用item,叫做common_user_item.xml</td>
	</tr>
  </tbody>
</table>
###4. drawable命名规范
<table>
    <thead>

	</thead>
    <tbody>
	 <tr>
	  <td>Button的背景图命名</td>
	  <td>
		图片：
		<table>
		 <tr>
		  <td>命名规范</td>
		  <td>状态</td>
         </tr>
		 <tr>
		  <td>图片名_normal或者直接图片名</td>
		  <td>(default state)</td>
         </tr>
		  <tr>
		  <td>图片名_pressed</td>
		  <td>state_pressed</td>
         </tr>
		  <tr>
		  <td>图片名_focused</td>
		  <td>state_focused</td>
         </tr>
		  <tr>
		  <td>图片名_disabled</td>
		  <td>state_enabled (false)</td>
         </tr>
		  <tr>
		  <td>图片名_selected</td>
		  <td>state_selected</td>
         </tr>
		 <tr>
		  <td>图片名_hovered</td>
		  <td>state_hovered</td>
         </tr>
		 <tr>
		  <td>图片名_checkable</td>
		  <td>state_checkable</td>
         </tr>
		 <tr>
		  <td>图片名_activated</td>
		  <td>state_activated</td>
         </tr>
		  <tr>
		  <td>图片名_windowfocused</td>
		  <td>state_windowfocused</td>
         </tr>
		</table>
	  </td>
	 </tr>
	 <tr>
	  <td>Button通用的shape命名</td>
	  <td>
		shape前缀规范：根据里面的属性来进行命名前缀,比如: btn_redff6d6d_radius2.xml， btn_redff6d6d_radius2_1strokef8f8f8_press.xml(如果项目里面已经有了调色板，整个系统button都使用统一的边框和红色或者其他颜色，可以进行简化,例如btn_red_press)
		<table>
		 <tr>
		  <td>命名规范</td>
		  <td>状态</td>
         </tr>
		 <tr>
		  <td>shape前缀_normal或者是直接shape前缀即可例如btn_red_radius2.xml</td>
		  <td>(default state)</td>
         </tr>
		  <tr>
		  <td>shape前缀_pressed</td>
		  <td>state_pressed</td>
         </tr>
		  <tr>
		  <td>shape前缀_focused</td>
		  <td>state_focused</td>
         </tr>
		  <tr>
		  <td>shape前缀_disabled</td>
		  <td>state_enabled (false)</td>
         </tr>
		  <tr>
		  <td>shape前缀_selected</td>
		  <td>state_selected</td>
         </tr>
		 <tr>
		  <td>shape前缀_hovered</td>
		  <td>state_hovered</td>
         </tr>
		 <tr>
		  <td>shape前缀_checkable</td>
		  <td>state_checkable</td>
         </tr>
		 <tr>
		  <td>shape前缀_activated</td>
		  <td>state_activated</td>
         </tr>
		  <tr>
		  <td>shape前缀_windowfocused</td>
		  <td>state_windowfocused</td>
         </tr>
		</table>
	  </td>
	 </tr>
	 <tr>
	  
	  <td>Fragment</td>
	  <td>fragment_模块名称.xml,例如：fragment_main.xml、fragment_user.xml</td>
	</tr>
 	 <tr>
	  <td>列表项</td>
	  <td>item_模块名称.xml</td>
	</tr>
    <tr>
	  <td>通用布局</td>
	  <td>common_布局的名称.xml，比如User的通用item,叫做common_user_item.xml</td>
	</tr>
	 <tr>
	  <td>selector</td>
	  <td>以selector结尾</td>
	</tr>
  </tbody>
</table>
###5. 编码命名规范
&ensp;&ensp;&ensp;&ensp;1. 类成员变量命名规范：android中的Activity，Fragment，Adapter和一些自定义View等以及包括一些业务处理的类（不包括model的属性）类成员变量命名规则如下所示：

	 public ImageView mIv_question;
	 public TextView mTv_car_num;

&ensp;&ensp;&ensp;&ensp;2. android组件类命名规范：

<table>
    <thead>
	 <tr>
	  <td>类</td>
	  <td>命名规范</td>
	 </tr>
	</thead>
    <tbody>
	 <tr>
	  <td>Activity</td>
	  <td>例如：主Activity叫做MainActivity</td>
	</tr>
 	 <tr>
	  <td>Adapter</td>
	  <td>例如：如果主Activity叫做MainActivity，那么Adapter叫做MainAdapter，取Activity的前缀</td>
	</tr>
    <tr>
	  <td>Fragment</td>
	  <td>例如：根据业务名称来命名（业务名Fragment）</td>
	</tr>

  </tbody>
</table>

###6. 代码注释规范
&ensp;&ensp;&ensp;&ensp;1.class头注释
	
   	/**
 	 * @ClassName: 类名（例如：MainActivity）
 	 * @Description: （类的描述）
	 * @Author (姓名，可以把写这个类的人的拼音或者英文名写入到这，通常android studio会根据系统用户名自动生成)
 	 * @Date: 2015/7/10 0010 （日期格式）
 	 */
如下模板可以通过打开android studio->settings->File and Code Templates中，打开Class设置项进行设置，把头部放入以下模板

	/**
	 * @ClassName: ${NAME}
	 * @Description: 
	 * @Author  ${USER}（如果系统有用户名可以用${USER}变量取，如果没有可以写死 用户名）
	 * @Date ${DATE}
	 */

&ensp;&ensp;&ensp;&ensp;2.方法注释

	/**
     * @Description:
     * @param datas  (参数描述)
     * @return  (返回值描述)
     */
##android注意事项
###1. Handler的使用
&ensp;&ensp;&ensp;&ensp;Handler机制有一个特点是不会随着Activity、Service的生命周期结束而结束。也就是说，如果你Post了一个Delay的Runnable，然后在Runnable执行之前退出了Activity，Runnable到时间之后还是要执行的。如果Runnable里面包含更新View的操作，程序崩溃了。

&ensp;&ensp;&ensp;&ensp;解决方案：

&ensp;&ensp;&ensp;&ensp;1.采用EventBus的开发方式，线程中的数据都可以通过消息的形式传到主Activity中。

&ensp;&ensp;&ensp;&ensp;2.采用[android-weak-handler](https://github.com/badoo/android-weak-handler),具体使用方式可以点击连接进行查看。

&ensp;&ensp;&ensp;&ensp;3.`@Override
    protected void onDestroy() {
        super.onDestroy();
        handler.removeCallbacksAndMessages(null);
    }`


###2. ListView的使用
&ensp;&ensp;&ensp;&ensp;1. 使用ListView时如果用到removeHeaderView，一定要确定ListView已经使用了setAdapter方法，不然会报NullPointException。

&ensp;&ensp;&ensp;&ensp;2. 如果ListView没有HeaderView或者FooterView的时候，与ListView相关联的Adapter就是传进来的参数Adapter。如果有，则原来的Adapter将被包装成HeaderViewListAdapter。

&ensp;&ensp;&ensp;&ensp;3. 使用ListView的addHeaderView时候，切记要放在setAdapter之前。由2可如果先setAdapter则与ListView想关联的Adapter是设置
的adapter，没有进行包装，在调用addHeaderView方法的时候会把adapter强制转换成HeaderViewListAdapter。这个时候就会报ClassCastException

&ensp;&ensp;&ensp;&ensp;4. 当我们使用给ListView添加了Header的时候，这个时候要注意，我们自定义adapter里面的getitem方法里面返回的position是不包括header的，也就是我们数据集合中的位置，而listview的onitemclick方法中返回的position是HeaderViewListAdapter中的位置，是带了header的。所以注意操作数据的时候记得-1

&ensp;&ensp;&ensp;&ensp;5. 使用ListView的时候，布局尽量使用fill_parent或者写死，如果使用wrap_content，它初始化的时候需要测量，会重复调用adapter的getView方法。在getView()方法中不要有实例化对象的操作。

###3. TabLayout的使用
&ensp;&ensp;&ensp;&ensp;在使用support-design包的时候偶然发现的问题(这玩意肯定是个bug，当时使用的版本是22.2.1):

		mViewPager.setAdapter(modelPagerAdapter);
        tabLayout.setupWithViewPager(mViewPager);
        for (int i = 0; i < titles.length; i++) {
            TabLayout.Tab tab = tabLayout.newTab();
            tab.setText(titles[i]);
            tabLayout.addTab(tab);
        }

&ensp;&ensp;&ensp;&ensp;一眼看去上面的代码是没有问题的，但其实不然，这样顺序会让tabLayout重复生成Title，如图所示：

&ensp;&ensp;&ensp;&ensp;![img](http://7xjwjf.com1.z0.glb.clouddn.com/git/android/Screenshot_com.coach.soft_2015-10-18-21-37-03_%E7%9C%8B%E5%9B%BE%E7%8E%8B.png?imageView2/2/w/300/q/100)  

&ensp;&ensp;&ensp;&ensp;正确顺序

		mViewPager.setAdapter(modelPagerAdapter);
        for (int i = 0; i < titles.length; i++) {
            TabLayout.Tab tab = tabLayout.newTab();
            tab.setText(titles[i]);
            tabLayout.addTab(tab);
        }
		tabLayout.setupWithViewPager(mViewPager);
##android小技巧
###1. SharedPreferences小技巧
&ensp;&ensp;&ensp;&ensp;SharedPreferences.Editor.commit这个方法是同步的，一直到把数据同步到Flash上面之后才会返回，由IO操作的不可控，尽量使用apply方法代替。apply只在API Level>=9才会支持，需要做兼容。
###2. ADB 命令技巧1
&ensp;&ensp;&ensp;&ensp;如果你用的是mac或者是linux再或者是windows上面得git shell，那么你就可以使用如下文件adb.sh,把下面的内容放入到adb.sh中，然后通过执行./adb.sh+空格+包名的形式去过滤定位到当前应用：


	#!/bin/bash
	packageName=$1
	pid=`adb shell ps | grep $packageName | awk '{print $2 }'`
	real_pid=`echo $pid | awk '{print $1}'`
	echo $real_pid+"#######"
	adb logcat | grep --color=auto $real_pid

###2. ADB 命令技巧2
&ensp;&ensp;&ensp;&ensp;当你发现你的adb命令不能使用或者是打不开的时候，可以试着采用如下命令去查看下是否有进程占用了你的端口：

&ensp;&ensp;&ensp;&ensp;linux or mac：

&ensp;&ensp;&ensp;&ensp;`netstat -ano | grep "5037"`

&ensp;&ensp;&ensp;&ensp;window：

&ensp;&ensp;&ensp;&ensp;`netstat -ano | findstr "5037"`

###3.string.xml技巧
&ensp;&ensp;&ensp;&ensp;在string.xml中定义html代码，可以采用如下的方式：

&ensp;&ensp;&ensp;&ensp;
```
    <string name='effect'>影响力：<![CDATA[<font color='#ff484a'>%1$s</font>]]></string>
```

&ensp;&ensp;&ensp;&ensp;在string.xml中使用空格可以通过代码 ```&#160;:&#160;```
去实现。

###4.android studio使用技巧
&ensp;&ensp;&ensp;&ensp;1. 检查无用的资源，在项目中点击右键，在出现的右键菜单中有“Analyze” --> “run inspaction by Name ...”。在弹出的搜索窗口中输入想执行的检查类型，如“Unused Resources”
##android兼容性bug
