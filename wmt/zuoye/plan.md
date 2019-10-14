# 作业数字化，大数据项目

## 用什么架构做服务器端 各客户端（皆用c++)
client: [https://github.com/mrtazz/restclient-cpp](REST client for C++)
Server&client: [https://github.com/eidheim/Simple-Web-Server](Simple-Web-Server)

## 实现

### 定时更新题目
    1. 由qml 定时锁要题目 (更新题目内容)
    2. 由另个一个控件给ui答案，给的方式
        １，要让ui产生变化
        ２，要产生一个信号，C++处理提交答案

### js　与 qml 合构成的组件
    6. 调时器元素使用javascript 代码

        调用js文件的介绍：
        https://blog.csdn.net/gongjianbo1992/article/details/88406655
        import "xxx.js" as Js

    5. 给qt界面下个定时器元素
        定时器的作用是：1.定时trigger某段js代码，或者改变某个元素的值
        

    4. 模块定义好后，要用到它，是怎么用的
        模块中的propery, 要给ui中的textField进行binding.
        模块的别名（as xxx) \
        在qml文件中执行为text = data.QtObjectId.property

    3. 定义模块的方法
        1. 模块定义文件的名字是qmldir
        2. 模块是以目录为单位，
            把某个模块的定义（qmldir)放在某个模块目录中
            把某个模块的API（*.qml)放在某个模块目录中
        3. 模块定义格式：　单例类型否 模块名　版本号　对应的qml文件(quick文件) 
        以上模块都应放在imports目录下，这样项目中的import 才会found.

    2. 交互模拟实验
        １：辨认
        ２：一个项英文单词
        ３：４个中翻译
        以上，可以转变为一个中文，找它对应的翻译

    1. qds (Qt design studio )  搭建一个UI
        就三个框：1,训练方法　2.题目　3.答题

## 愿境
1, 所有作业都在网上（数字化）
    实验：
        快速布题
        先定义正确答案
        题目的呈现 
            (先设计呈现和答题方式，才能设计软件架构)
    软件系统结构(能想到的，不能想到的，最好把所有的问题抽象出)
        规化好数据库
        规化好框架，功能穿插自如（模块组合）

2, 所有题型都用键盘作答（将来有更多，更人性化的交互）

3, 副功能(统计作业时间，统计错题)

## 呈现和答题方式 
    注：qt分开界面框架设计。代码框架另外完成
    从最基本的交互方式，逆行向上－－－从简到繁
        Qt有个状态机 --- 处理UI的逻辑关系
        qml的开发与调试

    设计框架：
        1.交互围绕掌上键盘设备：
            在程序中按不同的键，执行不同的动作
            点击动作：（换成组件激活的快捷键）
            输入动作：


