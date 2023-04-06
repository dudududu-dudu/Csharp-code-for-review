#Csharp-code-for-review
Starting level practicing
namespace variable;
class Program
{
    //static void Main(string[] args)
    //{
    //char a = 'c';
    //int b = a;
    //int b = 'a' 输出结果是a对应的97，不加特定''符号的话是根据上述逻辑等于99

    //int a = 50;
    //char b = (char)a;

    /*整数类容器强制放入字符串小容器内，需要强制转换（char）
     强制类型转换需要注意数字范围不能超出该容器范围否则回损失
     对照课件ASCII字符代码表
     */
    //char a = '\n';       
    //char b = '\\';
    //char c = '\"';
    //char d = '\t';
    //char e = '\'';
    //特殊字符转义，这里的\代表后面的特殊意义，a换行，两个\\代表一个\等

    //Console.WriteLine(a);
    //Console.WriteLine(b);
    //Console.WriteLine(c);
    //Console.WriteLine(d);
    //Console.WriteLine(e);

    //Console.WriteLine("c:\\a\\b\\c");
    //Console.WriteLine(@"c:\a\b\c");
    //Console.WriteLine(@"c:\\a\\b\\c");
    //在""前加上特殊字符@时后面就不需要\符号来进行转义，包括\n换行，\t缩进等操作
    //string str = @"www.sikiedu.com

    //siki";
    //string qaz = "www.sikiedu.com\n\nsiki";
    //声明字符串
    //Console.WriteLine(str);
    //Console.WriteLine(qaz);
    //输出字符串可以直接打印结果或者声明对象

    //string str2 = "123" + "456";
    //string str3 = str2 + "www";

    //Console.WriteLine(str2);
    //Console.WriteLine(str3);
    //字符串的相加是直接进行拼凑


    //String str = Console.ReadLine();
    //让控制台读取这一行输入，然后把这一行输入作为一个字符串返回给定义
    //Console.WriteLine(str +'q');

    //int a = Console.ReadLine();
    //赋值原则 1，类型一致 2，右边的值所需容器大小 小于左边的容器，此处类型不一致



    //Convert.ToInt32()

    //String str = Console.ReadLine();
    //从控制台输入数据此粗的直接定义是字符串
    //如果想输出的不是字符串而是可以做运算的数字，则需要转换数据类型
    //int strInt = Convert.ToInt32(str);
    // 将上面读取的字符串数据str转换成整数Int格式

    //int a = Convert.ToInt32(Console.ReadLine());
    //从控制台输入一个整数，然后返回给a赋值（最基本的直接以整数Int整数的数字进行输入）


    //不能转换，而且会报错，异常
    //Console.Write(strInt +"+"+ a+"=");Console.Write(strInt + a);
    //这里是转换后的整数的一个加减符号，后面接运算结果（简单的加法计算器）



    //int a = Convert.ToInt32(Console.ReadLine());
    //int b = Convert.ToInt32(Console.ReadLine());

    //Console.WriteLine(a+b);
    //Console.WriteLine((a + b) / 2);


    //从此处开始重新写一遍
    public static void Main(string [] args)
    {

        double a = Convert.ToDouble(Console.ReadLine());
        double b = Convert.ToDouble(Console.ReadLine());

        Console.WriteLine(a/b);


    }
}

