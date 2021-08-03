## C++ is_sorted()函数
在使用该函数之前，程序中必须先引入此头文件：#include <algorithm>

is_sorted() 函数有 2 种语法格式，分别是：
  
1. //判断 [first, last) 区域内的数据是否符合 std::less<T> 排序规则，即是否为升序序列。
  bool is_sorted (ForwardIterator first, ForwardIterator last);  
2. //判断 [first, last) 区域内的数据是否符合 comp 排序规则。
bool is_sorted (ForwardIterator first, ForwardIterator last, Compare comp);
