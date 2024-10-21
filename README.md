# 2024090914022-赖伊卡-CS-01
## 第一个程序
### 1.高级与低级语言的优劣
高级语言更加接近人类语言或者说是数学语言，让我们可以更加高效的编写代码，且具有较好的跨平台移植性，但执行效率相对较低，因为需要被编译或解释为低级语言且对于硬件的控制能力相对较弱。而低级语言则更加接近计算机硬件，能够被计算机直接识别和执行，自不待言，其执行效率会更高，且对于硬件的控制能力强。同时其可移植性比较差，且比较复杂。

对于我个人，会更喜欢低级语言，喜欢走进最底层的逻辑中。虽然目前仅能从基础开始，但以后会对低级语言进行了解与学习。
### 2.对于hello.c的逐行解读
    1.该行代码是一个预处理指令，它告诉编译器在实际编译之前要使用标准输入输出库stdio.h的内容。这个库提供了进行输入输出操作的函数，即库函数。
    2.这行代码定义了程序的入口点，即主函数，也就是程序执行中最先开始的函数。int表明这个函数的返回值为整数。
    3.这行代码调用了printf()函数，它是stdio.h库中定义的一个函数，用于格式化的输出。这里它输出字符串"Hello, world!"。
    4.这行代码表示main函数的结束，并向操作系统返回了一个整数值0。0通常也代表成功。
    5.大括号，标记函数结束。
### 3.可以删除哪一行
    return 0;行。虽然主函数是由int定义了返回值，但硬要删去该行不会影响结果。
### 4.
是储存整数。
因为main函数需要返回一个整数值给操作系统，以表示程序的退出状态。
### 5.
```c
#include <stdio.h>

int main() {
    printf("Hello glimmer!\n");
    return 0;
}
```
![image](https://github.com/Taylor-Lai/Glimmer-CS--easy---1-/blob/main/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-10-21%20183552.png)
 
## 基础语法运用
```c
#include <stdio.h>

int main() {
    int code;
    for(;;)
    {
		printf("Show me your code,please.\n");
        scanf("%d",&code);
        if(code >= 100000 && code <= 999999)
        {
            printf("I am super hacker!\n");
            break;
        }
        else
        printf("Fake code!\n");
    }
    return 0;
}
```

## 课后题
```c
#include <stdio.h>

int gcd(int m,int n)
{
    while(n!=0)
    {
        int a=n;
        n=m%n;
        m=a;
    }
    return m;
}
int main()
{
    int m,n;
    scanf("%d %d",&m,&n);
    int result =gcd(m,n);
    printf("%d\n",result);
    return 0;
}
```
