# gobang

该程序实现HTML五子棋
其中canvas.html通过canvas方式实现，dom.html通过dom操作实现五子棋程序

## 简要说明

### DOM方法实现
- `whoIsWinner()`、`judge()`、`chessArrayInit()`函数， 为DOM实现、Canvas实现的共同方法。
- `playAgain()` 函数 思路是一样的，有些许改变。
- `createBoard()` 函数 在DOM实现中，是通过DOM调用`createElement()`函数，来不断创建节点，达到创建棋盘的作用。
- `play()` 函数，在节点上进行`onclick()`监听，点击后在该节点绘制相应颜色的棋子。并赋值给chessArray二维数组。

### Canvas方法实现
- `whoIsWinner()`、`judge()`、`chessArrayInit()` 函数， 为DOM实现、Canvas实现的共同方法。
- `playAgain()` 函数 思路是一样的，有些许改变。只能开始，不能重新开始。
- `createBoard()` 函数 在Canvas实现中，是通过`getContext()`函数获取上下文，通过划线的方式来得到棋盘。
- `play()` 函数，监听鼠标事件，获取鼠标的坐标后进行计算。 
