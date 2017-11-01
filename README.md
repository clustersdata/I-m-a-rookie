# I-m-a-rookie

I'm a rookie

Problem Description
我是一只小菜鸟，都是笨鸟先飞，我想来个菜鸟先飞，我从0点出发一开始的飞行速度为1m/s，每过一个单位时间lin2144的飞行速度比上一个单位时间的飞行速度快2m/s，问n (0 < n < 10^5)个单位时间之后lin2144飞了多远?

Input

输入一个T表示为有几组数据

每组数据输入一个n，表示lin2144飞行的时间.

Output

输出我飞行了多远，因为数字很大，所以对10000取模.

Sample Input

2 1 2

Sample Output

1 4

代码：

#include<stdio.h>

int main()

{

    int t;
    
    __int64 n,k;
    
    scanf("%d",&t);
    
    while(t--)
    
    {
    
        scanf("%I64d",&n);
        
       
		k=n*n;
    
		if(k>10000)
    
			printf("%I64d\n",k%10000);
      
		else
    
			printf("%I64d\n",k);
      
    }
    
    return 0;
    
}

