---
title: My first COde
date : 2021-4-1
tags:
  - code
---
[AC code](https://vjudge.net/solution/29308044)
**題目簡述:**
鍵盤打字時，都剛好不小心往右打了一格，將它還原
**想法:**
用陣列建對應表，用if做對應表太冗(且不易閱讀)
``` cpp=
#include<iostream>
using namespace std;
char t[]={"`1234567890-=QWERTYUIOP[]\\ASDFGHJKL;'ZXCVBNM,./"};
int main(){
	char a;
	while((a = getchar()) != EOF){ 
			if(a==' '||a=='\n')putchar(a);
			else{
				int j;
				for(j=0;t[j]!=a;j++);
				putchar(t[j-1]);
			}
	}
}
```
**心得:**
原先是使用getline，但後來發現換行符號會被吃掉導致WA，似乎還沒有string可以接收'\n'還能輸出的函式，只好回去用char讀取輸出
**輸入相關語法整理:**

[2020一中資訊社寒訓05：字串與IO](https://docs.google.com/presentation/d/1BsM0YxfVeavMv0_tLMll524OggXQ86LBK2MTISa5xx4/edit#slide=id.p)
摘要:[C++裡getline()、get()、cin、getchar區別](https://www.itread01.com/content/1542222967.html)

