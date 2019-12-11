# java-note

ArrayList 时间复杂度和空间复杂度 链接（https://blog.csdn.net/u013030086/article/details/84967258）
1. ArrayList是实现了基于动态数组的数据结构，LinkedList基于链表的数据结构。
2. 对于随机访问get和set，ArrayList觉得优于LinkedList，因为LinkedList要移动指针。

ArrayList 是线性表（数组 )

    get() 直接读取第几个下标，复杂度 O(1)
    add(E) 添加元素，直接在后面添加，复杂度O（1）
    add(index, E) 添加元素，在第几个元素后面插入，后面的元素需要向后移动，复杂度O（n）
    remove（）删除元素，后面的元素需要逐个移动，复杂度O（n）

LinkedList 是链表的操作  

    get() 获取第几个元素，依次遍历，复杂度O(n)
    add(E) 添加到末尾，复杂度O(1)
    add(index, E) 添加第几个元素后，需要先查找到第几个元素，直接指针指向操作，复杂度O(n)
    remove（）删除元素，直接指针指向操作，复杂度O(1)

　　可以这样说：当操作是在一列数据的后面添加数据而不是在前面或中间,并且需要随机地访问其中的元素时,使用ArrayList会提供比较好的性能；当你的操作是在一列数据的前面或中间添加或删除数据,并且按照顺序访问其中的元素时,就应该使用LinkedList了。

java的常见类型转换



    //Int型数字转换成String
          int num1=123456;
          //方法1
          String str1=num1+"";  
          System.out.println(str1);
          //方法2
          String str2=String.valueOf(num1);    
          System.out.println(str2);
         
        //String转换成Int型数字
         String str3=new String("9876543");
         int num2=Integer.parseInt(str3);
         System.out.println(num1+num2);
        
         //字符转换成字符型数组
         String str4="HRuinger";
         char a[]=str4.toCharArray();
         for(int i:a)
           System.out.print((char)i+" ");
           System.out.println();
          
         //字符型数组转换成字符串
         char b[]={'H','R','u','i','n','g'};
         String str5=String.valueOf(b);
         System.out.println(str5);
         
         //整型与字符型数值的转换
         char c='3';
         System.out.println(c-'0');     //此处也可以为c-48
         int d=5;
         System.out.println((char)(d+'0'));    //此处也可以为c+48
         
 
 
@override 子类重写了父类的方法
应该坚持使用，养成编程习惯
