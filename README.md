# zuoye5
实验目的：
1.掌握字符串String及其方法的使用；
2.掌握文件的读取/写入方法；
3.掌握异常处理结构。

实验内容：
在某课上,学生要提交实验结果，该结果存储在一个文本文件A中。
文件A包括两部分内容：
一是学生的基本信息；
二是学生处理后的作业信息，该作业的业务逻辑内容是：利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能方法，实现如下功能：
1.每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
2.允许提供输入参数，统计古诗中某个字或词出现的次数
3.输入的文本来源于文本文件B读取，把处理好的结果写入到文本文件A
4.考虑操作中可能出现的异常，在程序中设计异常处理程序
输入：汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续>
输出：
汉皇重色思倾国，御宇多年求不得。
杨家有女初长成，养在深闺人未识。
天生丽质难自弃，一朝选在君王侧。
回眸一笑百媚生，六宫粉黛无颜色。
春寒赐浴华清池，温泉水滑洗凝脂。
侍儿扶起娇无力，始是新承恩泽时。
云鬓花颜金步摇，芙蓉帐暖度春宵。
春宵苦短日高起，从此君王不早朝。
…………

实验要求：
1.设计学生类（可利用之前的）；
2.采用交互式方式实例化某学生；
3.设计程序完成上述的业务逻辑处理，并且把“古诗处理后的输出”结果存储到学生基本信息所在的文本文件A中。

实验过程：
（1）在Student中定义name和Class和ID变量，定义构造方法Student，接受参数并在构造函数里调用各个set函数来设置各个变量的值。
（2）在Student中重写toString方法，用来返回对象的基本信息的字符串。
（3）在readTxt中导入各个包，如java.util.ArrayList，java.io.File包，定义静态变量字符串q，b和字符串型数组a。
（4）定义返回字符串方法readTxt接收参数为String类型的filePath，这个参数是在see3类中接收要处理的那个文本，创建File类型的file变量接收参数为filePath，用if来判定文件是文件时就返回返回true，只要存在就返回true方法为isFile，还有一个方法来判定不管他是不是文件只要存在就返回true，方法为exists。用InputStreamReader来接收要处理的文本。
（5）定义String类型的List，用数组lineTxt来接收从文本中读取的每行，用while来循环当读取的为null时跳出循环，这一就是实现了将文本中的东西存到了字符串中。

实验结果：
请输入学生姓名:依木拉
请输入学生学号:2019311574
请输入学生年龄:21
请输入学生性别:男
汉皇重色思倾国,御宇多年求不得。
杨家有女初长成,养在深闺人未识。
天生丽质难自弃,一朝选在君王侧。
回眸一笑百媚生,六宫粉黛无颜色。
春寒赐浴华清池,温泉水滑洗凝脂。
侍儿扶起娇无力,始是新承恩泽时。
云鬓花颜金步摇,芙蓉帐暖度春宵。
春宵苦短日高起,从此君王不早朝。
承欢侍宴无闲暇,春从春游夜专夜。
后宫佳丽三千人,三千宠爱在一身。
金屋妆成娇侍夜,玉楼宴罢醉和春。
姊妹弟兄皆列士,可怜光采生门户。
遂令天下父母心,不重生男重生女。
骊宫高处入青云,仙乐风飘处处闻。
缓歌慢舞凝丝竹,尽日君王看不足。
渔阳鼙鼓动地来,惊破霓裳羽衣曲。
九重城阙烟尘生,千乘万骑西南行。
<未完，待续>

实验感想：
此次实验让我更加了解了文本的读取与写入方法，字符串String及其方法的使用，异常处理等结构方法。让我深入的了解了他们，对他们有更深层次的认识，也对Java语言有了更深刻的理解。
学会了Scanner的next和nextInt方法的区别，是输入字符串和整形，复习了toString的用法，返回字符串对象，学会建立BufferedReader新的对象读取文件，建立PrintWriter新的对象写入文件，用indexOf方法查找字符串中指定字符串
