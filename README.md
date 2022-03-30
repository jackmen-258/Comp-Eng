## Hello Github!
#### Hello Markdown!
[Markdown教程](https://www.runoob.com/markdown/md-tutorial.html)

跳转至:[FILE2.md](https://github.com/jackmen-258/Comp-Eng/blob/main/FILE2.md)

image in the directory:![alt star sky](https://raw.githubusercontent.com/jackmen-258/Comp-Eng/main/1.jpg)

image in the web:![alt The Grand Budapest Hotel](https://pic2.zhimg.com/v2-d2a555c7e7328a0e0dd489f9a4713732_1200x500.jpg)

Eight queens:
```C++
#include <iostream>
#include <algorithm>
#include <bitset>
#include <numeric>
#include <utility>
int main() {
  for (int queens[] = {0,1,2,3,4,5,6,7}; ::std::next_permutation(queens,queens+8); )
    if ((::std::bitset<15>(::std::accumulate(queens,queens+8, ::std::make_pair(0, 0), [](::std::pair<int, int> a, int b){return ::std::make_pair((1<<(b+a.second))|a.first,a.second+1);}).first).count() == 8) && (::std::bitset<15>(::std::accumulate(queens, queens+8, ::std::make_pair(0, 0), [](::std::pair<int, int> a, int b){return ::std::make_pair((1<<(7+b-a.second))|a.first, a.second+1);}).first).count() == 8))
      ::std::cout << queens[0] << queens[1] << queens[2] << queens[3] << queens[4] << queens[5] << queens[6] << queens[7] << ::std::endl;
}
```

> 你  
> 一会看我  
> 一会看云  
> 我觉得  
> 你看我时很远  
> 你看云时很近  

+ 数据结构
+ 计算机组成原理
+ 操作系统
+ 计算机网络

1. 张三
2. 李四
3. 王五

|  省份   |  地区生产总值 |
| :----:  | :----------: |
|   广东  |   124369.67  |
|   江苏  |   116364.2   |
|   山东  |   83095.9    |

**bold text**  
*italicized text*  
~~strikethrough text~~  

---