---
title: My first COde
date : 2021-4-1
tags:
  - code
---
[AC code](https://vjudge.net/solution/29308044)
**�D��²�z:**
��L���r�ɡA����n���p�ߩ��k���F�@��A�N���٭�
**�Q�k:**
�ΰ}�C�ع�����A��if��������Ӥ�(�B�����\Ū)
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
**�߱o:**
����O�ϥ�getline�A����ӵo�{����Ÿ��|�Q�Y���ɭPWA�A���G�٨S��string�i�H����'\n'�ٯ��X���禡�A�u�n�^�h��charŪ����X
**��J�����y�k��z:**

[2020�@����T���H�V05�G�r��PIO](https://docs.google.com/presentation/d/1BsM0YxfVeavMv0_tLMll524OggXQ86LBK2MTISa5xx4/edit#slide=id.p)
�K�n:[C++��getline()�Bget()�Bcin�Bgetchar�ϧO](https://www.itread01.com/content/1542222967.html)

