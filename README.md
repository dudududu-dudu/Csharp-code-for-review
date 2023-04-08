#Csharp-code-for-review

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


        double a = Convert.ToDouble(Console.ReadLine());
        double b = Convert.ToDouble(Console.ReadLine());

        Console.WriteLine(a/b);
//  &&和  ||或   !非
        bool a = (3 < 4) && (9 < 10);// true && false

        bool b = (3 < 2) && (9 < 7);

        bool c = !(4 < 7);

        Console.WriteLine(a);
        Console.WriteLine(b);
        Console.WriteLine(c);

        //输入一个人的年龄，判断这个是否为青壮年，青壮年的标准是18-60岁


        int age = Convert.ToInt32(Console.ReadLine());
        
        bool isYoung = (18 <= age) && (age<=60);

        Console.WriteLine(isYoung);
        
        int mathScore = Convert.ToInt32(Console.ReadLine());
        int englishScore = Convert.ToInt32(Console.ReadLine());
        bool award = mathScore >= 90 && englishScore >= 90;
        bool award2 = !(mathScore < 90) && !(englishScore < 90);
        Console.WriteLine(award);
        Console.WriteLine(award2);
        
        

     /* 加法+
         * 减法-
         * 乘法*
         * 除法/
         * 取模（求余）%  注意用于整数，小数容易不精确
         */
        //问题....设计一个算法，可以吧任意一个两位数分离它的个位和十位上面的数字
        //比如78，十位是7，个位是8,且运用格式化输出,同时使用输入指令
        //Convert.ToInt32(Console.ReadLine());

        int a = Convert.ToInt32(Console.ReadLine());
        int shi = a / 10;
        int ge = a % 10;
        
        Console.WriteLine(a+"的十位是{0},个位是{1}",shi,ge);
        //注意此处的逻辑符号,""外面的+代表数字和内部字符串的合并后面的,是格式化后应用的数据
        //赋值运算符 +=, -=, *=, /= 将左边的数用等号前面的符号和右边数字进行运算

        int x = 1;
        x += 10; //x = 1 + 10 = 11
        x -= 11; //x = 11 - 11 = 0
        Console.WriteLine(x);


        int p = 7;
        p /= 3; //p =7/3=2
        p *= 3; //6
        Console.WriteLine(p);
        
        
        
        int number = Convert.ToInt32(Console.ReadLine());
        if (number % 2 == 1)//这里的条件语句是逻辑判断所以是两个==等号
        {
            Console.WriteLine("奇数");
        }
        else
        {
            Console.WriteLine("偶数");
        }
    
        int Score = Convert.ToInt32(Console.ReadLine());
        if (Score >= 90)
        {
            Console.WriteLine("A");
        }
        else if (Score >= 70)
        {
            Console.WriteLine("B");
        }
        else if (Score >= 60)
        {
            Console.WriteLine("C");
        }
        else if(Score>=0)
        {
            Console.WriteLine("D");
        }
        int x = Convert.ToInt32(Console.ReadLine());
        int y = Convert.ToInt32(Console.ReadLine());

        if (x > 0 && y > 0)
        {
            Console.WriteLine("位于第一象限");
        }
        else if (x < 0 && y > 0)
        {
            Console.WriteLine("位于第二象限");
        }
        else if (x < 0 && y < 0)
        {
            Console.WriteLine("位于第三象限");
        }
        else if (x > 0 && y < 0)
        {
            Console.WriteLine("位于第四象限");
        }
        else if (x == 0 && y != 0)
        {
            Console.WriteLine("位于y轴上");
        }
        else if (x != 0 && y == 0)
        {
            Console.WriteLine("位于x轴上");
