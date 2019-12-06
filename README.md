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
