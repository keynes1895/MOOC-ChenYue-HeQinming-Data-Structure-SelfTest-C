# twin-primes-conjecture
![题干](http://i4.eiimg.com/1949/c498762f04b47969.png)
```C
# twin-primes-conjecture
![题干](http://i4.eiimg.com/1949/c498762f04b47969.png)
​```C
#include <stdio.h>  
#include <stdlib.h>    
#include <math.h>  
int is_prime(int n) 
{  
    int i = 0;  
    for (i = 2; i <= sqrt(n); i++) {  
        if (n % i == 0)  
            return 0;  
    }  
    return 1;   
}  
int main()  
{  
    int n = 0, count = 0, i = 0, tmp = 1;  
    while (scanf("%d", &n) != EOF) {  
        for (i = 2; i <= n; i++) {  
            if (is_prime(i)) {  
                if (i - tmp == 2)  
                    count++;  
                tmp = i;  
            }             
        }  
        printf("%d\n", count);  
    }    
    return 0;  
}  
​```

```
