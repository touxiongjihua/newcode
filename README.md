# newcode
daimaduibi
.版本 2

.子程序 _启动窗口_创建完毕
.局部变量 计数, 整数型
计数 ＝ 0

' 设置窗口标题
窗口1.标题 ＝ “圣诞节快乐！”

' 初始化动画文本
编辑框1.内容 ＝ “🎄 圣诞节快乐！🎁”
编辑框2.内容 ＝ “”
计时器1.时间间隔 ＝ 300
计时器1.启动 ()

.子程序 计时器1_周期事件
计数 ＝ 计数 ＋ 1
感恩节的故事 🌽🦃🍂

在一个宁静的小镇上，感恩节快要到了。小女孩露西和她的家人正在忙着准备节日的盛宴。 🍽️🎉
露西决定做一些特别的事情，她想给每个人一个惊喜礼物。🎁✨

她走进森林，发现满地的落叶像是金色的地毯。🍁🍂忽然，她看见一只受伤的小火鸡躲在树丛里。🦃💔
“别怕，我会帮你！”露西轻轻地说道。她把火鸡带回家，和妈妈一起为它包扎伤口。她给它起名叫“幸运”。 🍀❤️

晚上，家人围坐在餐桌旁，桌上摆满了南瓜派、玉米和香喷喷的火鸡。🎃🌽🍗
就在大家准备感恩祈祷时，露西笑着抱着“幸运”走进房间。“今年我们不吃火鸡了，我们有了一位新朋友！”她大声宣布。 😊🦃🎉

家人们愣了一下，随即都笑了起来。他们为幸运留下了一个特别的位置，并分享了更多的爱与感恩。❤️🙏
窗外，星星闪烁，仿佛也在祝福这个充满温暖的小家。🌟🏡

感恩节的意义，不仅是享受美食，更是感恩生命中的每一份小确幸。 🌟🍂✨


' 制作简单动画效果
选择 (计数 % 3)
    情况 0
        编辑框2.内容 ＝ “✨🎄”
    情况 1
        编辑框2.内容 ＝ “🎁✨”
    情况 2
        编辑框2.内容 ＝ “✨🎅”
结束选择

' 增加循环祝福
如果 (计数 ＝ 20)
    编辑框1.内容 ＝ 编辑框1.内容 ＋ “🎉愿你新年快乐！🎊”
    计时器1.停止 ()
结束如果

  DDei是一个遵循Apache2.0开源协议开发的设计器组件，允许用户通过拖拉拽等方式创建和编辑图形。 使用者可以通过组件引用的方式，将其嵌入到应用的任意位置，使之拥有在线绘图的能力。

功能特性
  DDei以组件的方式提供使用，功能强大且易于集成，大多数功能都可以通过初始化配置和引入插件完成，无需复杂编码。以下是DDei的功能特性

画布大小

  支持设置设计器的大小。

背景

  支持空白、图片、纯色以及透明度设置。

纸张

  开启后会在背景上显示纸张。允许设置纸张的大小（如：A4、A5、自定义）以及方向（横向、纵向）。

标尺

  开启后会在绘图区域的周围显示标尺，同时会影响辅助网格的尺寸。支持毫米、厘米、米、英寸、像素等单位。

辅助对齐

  开启后拖拽时会显示对齐辅助线。

辅助网格

  开启后会在背景上绘制用于对齐的辅助网格线。支持点阵和网格两种类型。

水印

  开启后图形上方显示水印。支持文字、图像两种水印类型，可以调整水印的字体、文本、图片、方向、颜色和透明度。
2
无限画布

  开启后在操作超出画布大小时会自动扩展画布。可以限制扩展方向（横向或纵向）。

权限控制

  可以配置操作权限。支持全局只读设置，或到图形实例级的创建、修改、选择、删除、连线等权限。 多文件

  可以配置插件实现多文件编辑。

多页签

  可以配置插件实现多页签编辑。

多图层

  开启后可以创建多个图层，并在不同图层之间切换、锁定或删除图层。

数据驱动

  DDei采用数据驱动，图形的绘制与JSON模型绑定，图形操作和模型数据会相互同步。可以通过API获取图形的JSON数据，或通过已有的JSON数据显示加载画布。

插件机制   DDei提供了插件机制，使用者可以通过扩展插件对设计器功能进行装载或卸载。也可以通过自定义插件扩展个性化功能，从而满足使用需求。

安装、示例与API
  作者提供了完整的安装指南和示例，请进入DDei文档查看最新文档。

技术支持
QQ:3697355039     邮箱：3697355039@qq.com
