# myrime

我的 rime 配置文件

double_pinyin.custom.yaml --- 自然码双拼的自定义文件，适合安卓版 trime，不适合 windows 版小狼毫

weasel.custom.yaml --- Windwos 小狼毫输入法的主题皮肤自定义文件

xxx.trime.yaml --- 安卓 trime 同文输入法的主题皮肤文件，按照 trime 的版本号来下载对应文件夹里的主题

# 安卓主题说明

三个主题是按键大小的区别，功能是一样的。每个主题都有“彩、黑、黛、灰、白”五个颜色。

`通常，输入方案自带有中英切换，一般是用来切换 default 键盘的 ascii 状态，切换不到独立的 letter 键盘。`

`本主题（v3.2.19或以上版本）的中英按钮是切换 default 键盘和  letter 键盘，所以可以分别设置两个键盘的按键布局和长按符号。`

`两个切换按钮同时使用会有一点点交互上的小冲突，建议保留一个键盘上的中英切换就好了。`

增加了 [stroke](https://github.com/rime/rime-stroke) 和 [one_hand](https://gitee.com/yq-ysy/one-hand_-rime) 这两个笔画输入法布局，遇到不会拼音的生僻字，也是用得上的。个人觉得后者比较好用，虽然其实，他们比起大厂做的笔画输入，还是有差距的。

长按或下滑，就是输出按键右上角的数字或符号，可以编辑 xxx.trime.yaml 文件，自行设定上下左右各个方向的下滑功能。

打字出现候选字的时候，回车键左边的按键，会变成显示更多候选的按键。建议在设置里，把每页显示候选词的数量设定为 100，使用效果更佳。`注：trime 3.3.0 版本已经自带候选下拉按钮，这个已经不再需要`

点击符号按钮，中文模式时打开的就是中文符号键盘，英文模式时打开的就是英文符号键盘。


# one_hand 笔顺说明：

1、one_hand 笔顺的最小安装只需下载三个文件，下载地址：[one_hand](https://gitee.com/yq-ysy/one-hand_-rime)：

```
one_hand.schema.yaml

one_hand.dict.yaml

one_hand.text.dict.yaml
```

[也可以直接在这里下载](https://github.com/chwt163/mytrime/tree/main/one_hand%20%E7%AC%94%E9%A1%BA)

2、one_hand 笔顺没有对安卓的虚拟键盘做匹配优化，可以对 one_hand.schema.yaml 作一些更改，添加模糊音：

```
  algebra:
    - derive/^1/7/
    - derive/^2/8/
    - derive/^3/9/
    - derive/^4/6/
    - derive/^5/0/
```

3、one_hand 笔顺有三个词库文件，其中两个体积比较大，个人觉得保留单字就足够了，可以在 one_hand.dict.yaml 里面注释掉：

```
import_tables:
  - one_hand.text                 # 单字及标点符号数字序号，20988个汉字
  #- one_hand.guanjian             # 关键词库，54万——很大
  #- one_hand.changyong            # 常用词汇短语，192万——特大
```

# 截图：

![常规-彩色](https://github.com/user-attachments/assets/0036136b-1074-422c-8307-f1c6d1e3a759)


![常规-白色](https://github.com/user-attachments/assets/441c4d3f-72fd-4a5c-9a54-fd3bd17522e4)


![常规-黑色](https://github.com/user-attachments/assets/7a7e2cd0-15e0-4d37-9aa5-1044d3cd7436)


![大大按键-彩色](https://github.com/user-attachments/assets/1cc3d15e-c45b-4270-857a-5d98ee88efa2)


![大大按键-灰色](https://github.com/user-attachments/assets/934d1039-eac3-4fe9-b9e2-912134588ea1)


![大大按键-黛色](https://github.com/user-attachments/assets/eee63f96-c8bf-4e3f-a597-faf401813ecd)


![笔顺](https://github.com/user-attachments/assets/bd8cad51-5a5f-4115-8518-f1cba0c4fd90)











