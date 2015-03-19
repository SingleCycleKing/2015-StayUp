#2015 Unique Studio Android Team Stay Up Examination (Part A)


#####Tip: If you are freshman, please finish the questions of part B. If you choose to finish the questions of part A, however, you can gain double scores. If you are sophomore, you must finish the questions of part A.


##1.Java Basic Question (10 Points)
- Please write a piece of code which can display the names of all the files and subfiles in the current folder and output it into a txt file.

##2.HTTP (15 Points)

- Please use following parameters to connect with remote service. And write down the HTTP request that the server socket will receive. <br/>
URL:http://hustunique.com:80/exgfs.json?from=1449803471000<br>
RequestProperty:"User-Agent", "UniqueStudio Spider"<br>
DATA:username=NIANTIC&password=Sk9JTiBUSEUgUkVTSVNUQU5DRSBJVCBJUyBUSU1FIFRPIE1PVkU
Tips:[HttpURLConnection](http://developer.android.com/reference/java/net/HttpURLConnection.html)

##3.Algorithm (20 Points)
> Date.Structure+Algorithm=Progarm

- The equation is the key to program.Tonight you will learn one of ADT and use it to solve one simple problem.(you can search any information through the internet)

- Binary Tree is an abstract data type.Just Like this.
![tree picture](http://upload.wikimedia.org/wikipedia/commons/thumb/d/df/Binary_tree.png/350px-Binary_tree.png)
For more information click [BinaryTree](http://zh.wikipedia.org/wiki/%E4%BA%8C%E5%8F%89%E6%A0%91)
What we will use tonight is only **the expression tree**.

- The Postfix Expression:
We often use **the infix expression** for calculation in daily life. Just like  **5+2*2=9**.
But it is easier for you to design a calculator using **the postfix expression**. We can transform the infix expression above into the postfix expression below.** 5,2,2,*,+**
For more information click [postfix expression](http://zh.wikipedia.org/wiki/%E9%80%86%E6%B3%A2%E5%85%B0%E8%A1%A8%E7%A4%BA%E6%B3%95)

####First Task
- Use C/C++ or Java to implement the binary tree and construct the expression tree below.
![expression tree](http://f.hiphotos.baidu.com/zhidao/pic/item/ac345982b2b7d0a251b12249cbef76094a369aed.jpg)
>  Hint for C
* linked list
* Warning for Java
* Do not use the built-in class like ArrayList...


####Second Task
implement the function below.(use the constructed tree in Task1)

```java
/**input :the head of the expression tree you have constructed in First Task
function: convert the expression tree into the postfix expression (you can directly print it)
the correct print: 3 2 3 * + 6 3 / -
*/
void convertTreeToPostfixExpression(...){...}
```
##4.Database (25 Points)


- 隔壁寝室老王（As a PM）最近拉到了风投，开了个交♂友论坛。
老王听说了你的能力，便请你来管理数据库。“嘛，我们钱多，要用就用最好的服务器，这些你就不用担心了。”，老王如是说道。半信半疑的你接受了他的邀请。老王的服务器现在跑的是MySql，字符集为Chinese_PRC_CS_AI(大小写敏感字符集)。

- 这是他们现在数据库里面的表：


- Table：user<br>uid：用户id，int型，自增<br>username：用户名，字符串

|&#8195;&#8195;&#8195;uid&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;username&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;|
|:-:|:-:|
|0|fhw|
|1|SingleCycle|
|2|Orz3969|
|3|Evsmuta|
|4|U201314444|
|5|U201314458|
|6|U201314477|

-
Table：thread<br>tid：帖子的id，int型，自增<br>tname：帖子的名字，字符串<br>creator：发帖人的id，int型

|&#8195;&#8195;&#8195;tid&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;tname&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;creator&#8195;&#8195;&#8195;|
|:-:|:-:|:-:|
|104|联创团队招新了|0|
|405|谁是团队最帅的人|3|

-
Table：reply_list<br>userid：回复的人的id，int型<br>postid：该回复在这个帖子中的id，int型<br>pcontent：回复的内容，字符串<br>tid：帖子的id，int型

|&#8195;&#8195;userid&#8195;&#8195;|&#8195;&#8195;&#8195;postid&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;&#8195;pcontent&#8195;&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;tid&#8195;&#8195;&#8195;|
|:-:|:-:|:-:|:-:|
|5|1|举爪|104|
|5|5|我|405|
|5|2|哈哈|104|
|2|6|你们别闹|405|
|6|7|是我|405|

- 请设计sql语句，创建上述表

- 老王觉得如果要赚钱，一定要先给土豪花钱的机会。一拍脑门，老王准备给网站加入会员系统。请给第一个表user加入一列rank，int类型

- 老王看到有一堆昵称类似于U201314XXX的用户，心里非常生气，他知道是他的室友来砸场子了。为了维护这个社区的逼格，老王决定删除这些用户。请你帮老王实现他的小愿望。（要求：限定只能用一句sql）

- 为了帖子的有序，也为了楼层功能的实现，帖子中的回复id（列postid）需要有自增功能，比如说，帖子id（列tid）为104的帖子有了新回复，下一次插入的postid便应该为3。用户“SingleCycle”向帖子id为405的帖子回复了新内容“哈哈”。（要求：限定只能用一句sql）

- Bad News（风投公司出现债务危机，老板携款和老王的女朋友跑了。老王在悲痛之余决定仍然把这个网站做下去。当然，现在我们可承受不起豪华的阿*云服务器，老王现在手里只有个树莓派，搭上服务器之后，数据库从MySQL也变成了SQLite。虽说抢救了部分数据，但是有些查询语句还是丢失了。老王又TM发现他的大学室友注册了账号来发帖了。请你设计SQL语句首先创建下列表单，再删除老王室友发送的帖子（注意47号不是他室友）

|&#8195;&#8195;&#8195;uid&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;username&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;|
|:-:|:-:|
|0|fhw|
|1|SingleCycle|
|2|Kami_Control|
|44|U201314444|
|45|U201314444|
|46|U201314477|
|47|u201314爱你一生一世|

|&#8195;&#8195;userid&#8195;&#8195;|&#8195;&#8195;&#8195;postid&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;&#8195;pcontent&#8195;&#8195;&#8195;&#8195;|&#8195;&#8195;&#8195;tid&#8195;&#8195;&#8195;|
|:-:|:-:|:-:|:-:|
|45|7|666|101201|
|45|8|666|101201|
|44|2|666|101454|
|44|5|666|108777|
|47|9|666|101201|

- 要求：删除操作限定只能用一句sql（）<br/>
Tip：MySQL和SQLite有不同的地方（）

##5.Android (30 Points)

- Please complete a simple music player. Here is what you need to accomplish.
- When user first opens the app, he will see the guide page which say "Hello". And when he opens the app again, it won't appear again.
- There is a listview to show all the music files in the sdcard. And when user click an item in the list, it will start an activity to play the music.
- The activity has two buttons. One of them is used to play or stop the music, and the other one is used to play next music.
- The music can be played in the background.
- Tip: [Here](http://hukai.me/android-training-course-in-chinese/)
