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
newssr
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
