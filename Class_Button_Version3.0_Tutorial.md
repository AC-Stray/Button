# Class Button Version3.0 Tutorial
## Information
Button3.0 by AbsoCube Studio

Button3.0 Update Log:

Update Time : 2020/2/21 Friday

Update Contents :

Remove redundant functions and add color_update.

Tutorial Writing Time : 2020/3/14 Saturday
## Usage
����ʹ��������д

��Class_Button��Դ�����£���ʹ��button��������һ������ʾ�����򣬿ɹ��ο�
### Create Instance
������Ҫ����һ��ʵ��������Ҫ���²�����

` posx, posy, length, width, text, bfont, color, textcolor=(0, 0, 0)`

(int)posx : ��ť���Ͻǵ�x����

(int)posy : ��ť���Ͻǵ�y����

(int)length : ��ť����

(int)width : ��ť���

(str)text : ��ť�ϵ�����

(pygame.font.Font)bfont : ��������

(tuple)color : ��ť��ɫ

(tuple/str)textcolor : ������ɫ��Ĭ��(0, 0, 0)��ɫ�����Դ��ݡ�opposite����
��ʹ���밴ť��ɫ�෴����ɫ

���ԣ��㴴����ʵ��������������

`change = button(20, 20, buttonlength, buttonwidth, "change", pfont, (255, 255, 255), "opposite")`
### function : show
ʹ�ô˺��������ð�ť����Ļ����ʾ����
### function : pressed
��Ҫ���ݵĲ�����

`event`

(pygame.event.get)event : �¼�����������¼����м�⣬���������˰�ť������True

��Ĵ��������������
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
�����ڴ���ʵ����԰�ť��ɫ�������޸ģ����ܻ������ɫδ�ı������ɫ����������
ʹ�ô˺������Զ԰�ť��ɫ���и���
## Ending
This is the end of the tutorial.
Please contact me if you have any problems using it or have some advise.

The following is my contact information:

QQ : 1684671388

Email : absocube@qq.com

GitHub : github.com/AC-Stray