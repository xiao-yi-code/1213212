# 1213212

int main()
{
	extern int flae;//extern声明外部符号,表示外部有一个定义好的flae,在这里什么一下就可以直接用了
	printf("flae=%d\n",flae);
  return 0;
}

void test()
{

	//static修饰局部变量时，局部变量的生命周期变长
	//static修饰全局变量时，改变了变量的作用域，让静态的全局变量只能在自己所在的源文件内部使用，出了源文件就不能使用了
    static int a = 1;//是一个静态的局部变量
	a++;
	printf("a=%d\n",a);
}
int main()
{
	int i = 0;
	while(i<5)
  {
	test();
	i++;
  }
 
 
 return 0;
}
