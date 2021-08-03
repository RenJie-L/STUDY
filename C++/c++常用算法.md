## C++ is_sorted()函数
在使用该函数之前，程序中必须先引入此头文件：`#include <algorithm>`

is_sorted() 函数有 2 种语法格式，分别是：
  
1. //判断 [first, last) 区域内的数据是否符合 std::less<T> 排序规则，即是否为升序序列。  
  `bool is_sorted (ForwardIterator first, ForwardIterator last);  `
2. //判断 [first, last) 区域内的数据是否符合 comp 排序规则。  
`bool is_sorted (ForwardIterator first, ForwardIterator last, Compare comp);`
其中，first 和 last 都为正向迭代器（这意味着该函数适用于大部分容器），[first, last) 用于指定要检测的序列；comp 用于指定自定义的排序规则。
> 注意，如果使用默认的升序排序规则，则 [first, last) 指定区域内的元素必须支持使用 < 小于运算符做比较；同样，如果指定排序规则为 comp，也要保证 [first, last) 区域内的元素支持该规则内部使用的比较运算符。  

  另外，该函数会返回一个 bool 类型值，即如果 [first, last) 范围内的序列符合我们指定的排序规则，则返回 true；反之，函数返回 false。值得一提得是，如果 [first, last) 指定范围内只有 1 个元素，则该函数始终返回 true。                                                                  
