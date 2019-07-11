# 牛顿迭代法求N的平方根

```c++
double x=10;//猜一个近似的数
double n=5;
while(1){
  cout<<x<<endl;
  if(x==(x+n/x)/2)break;
  x=(x+n/x)/2;
}	
```

