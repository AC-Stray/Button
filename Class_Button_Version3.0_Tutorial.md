# Class Button Version3.0 Tutorial
## Information
Button3.0 by AbsoCube Studio

Button3.0 Update Log:

Update Time : 2020/2/21 Friday

Update Contents :

Remove redundant functions and add color_update.

Tutorial Writing Time : 2020/3/14 Saturday
## Usage
以下使用中文书写

在Class_Button的源代码下，有使用button类制作的一个简易示范程序，可供参考
### Create Instance
当你想要创建一个实例，你需要以下参数：

` posx, posy, length, width, text, bfont, color, textcolor=(0, 0, 0)`

(int)posx : 按钮左上角的x坐标

(int)posy : 按钮左上角的y坐标

(int)length : 按钮长度

(int)width : 按钮宽度

(str)text : 按钮上的文字

(pygame.font.Font)bfont : 文字字体

(tuple)color : 按钮颜色

(tuple/str)textcolor : 文字颜色，默认(0, 0, 0)黑色，可以传递“opposite”，
会使用与按钮颜色相反的颜色

所以，你创建的实例会类似这样：

`change = button(20, 20, buttonlength, buttonwidth, "change", pfont, (255, 255, 255), "opposite")`
### function : show
使用此函数，会让按钮在屏幕上显示出来
### function : pressed
需要传递的参数：

`event`

(pygame.event.get)event : 事件，函数会对事件进行检测，如果鼠标点击了按钮，返回True

你的代码会类似这样：
```        
for event in pygame.event.get():
if event.type == QUIT:
    sys.exit()
if change.pressed(event):
    randomcolor = random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)
    change.color = randomcolor
    change.color_update()
```
### function : color_update
当你在创建实例后对按钮颜色进行了修改，可能会出现颜色未改变或是颜色出错的情况，
使用此函数可以对按钮颜色进行更新
## Ending
This is the end of the tutorial.
Please contact me if you have any problems using it or have some advise.

The following is my contact information:

QQ : 1684671388

Email : absocube@qq.com

GitHub : github.com/AC-Stray