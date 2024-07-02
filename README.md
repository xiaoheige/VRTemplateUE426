# UE4 VR Template

## 封装内容：

**1.手部模型**

要更换VRHands目录下的其他手模型，只需打开BP_MotionController，选中HandMesh，修改Details栏中的Animation下的Anim Class项

**2.右手射线**

用Spline实现。粒子实现方式有问题，射线隐藏后，vrpawn隔着actor移动，再显示不出来了

**3.手部提示框**

含StepName变量，可播放声音

**4.UI Demo**

**5.高亮显示**

两种方式：设置PostProcessVolume和更换材质。使用说明：把BPBaseFunc蓝图类放到场景中即可使用HighlightActor和UnhighlightActor两个方法

https://zhuanlan.zhihu.com/p/455073329

https://zhuanlan.zhihu.com/p/337393342

**6.操作键重新规划**

**7.更换手套**

**8.Demo场景**

**9.Start场景**

含手柄操作说明和场景选项

**10.中文字体**

使用字体：场景中选择中TextRender项，Details中的Text下的TextMaterial和Font选择自定义的字体和材质球。

添加字符集：修改Font里的ImportOptions下的Chars，点击Asset菜单下的ReimportFont以重新导入字体并保存。修改对应的材质球，把FontParam的Font项清空再重新选择刚修改的Font，保存材质。

创建新字体：修改Font里的ImportOptions下的FontName和Height(字号)，下边的操作参照如上“添加字符集”。

**11.用interface实现Actor被抓取、放开事件触发**

**12.研究怎么把处置流程串成一条线**

点击、菜单选择、triggerbox等
**13.选择菜单**

**14.模拟JS按钮点击事件**

蓝图通过Event Dispatcher实现

**15.文字版按钮也采用Menu的按钮**

**16.设置LOGO**

**17.手柄移动范围显示**


## todo:

- 优化SetTips方法，播放完声音自动继续执行（没有声音的时候直接继续执行）

- 考虑把stepname独立出来


**说明：转用UE5，该框架暂停更新！**
