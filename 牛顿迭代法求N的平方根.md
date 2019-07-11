# 牛顿迭代法求N的平方根

```c++
public:
    int mySqrt(int x) {
        if(x>=2147395600)return 46340;
        if(x==0)return 0;
        double n=1;
        while(abs(-n+x/n)/2>=1e-6){
            n=(n+x/n)/2;
        }
        return n;
    }
};
```

