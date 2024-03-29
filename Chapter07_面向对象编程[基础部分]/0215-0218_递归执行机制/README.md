# 0215-0218_递归执行机制

```java
//省略调用部分，n = 4。
public void test(int n)
{
	if(n > 2)
	{
		test(n - 1);
	}
	System.out.println("n = " + n);
}
```

![递归执行机制01.jpg](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F4b165318-6383-451c-8845-110b786c9f0a%2F0d8e42a8-4001-4a1b-af62-76edfb0d604c%2F%25E9%2580%2592%25E5%25BD%2592%25E6%2589%25A7%25E8%25A1%258C%25E6%259C%25BA%25E5%2588%25B601.jpg?table=block&id=d097c0ee-e725-4a9c-9b5d-36b652e72ad8&t=d097c0ee-e725-4a9c-9b5d-36b652e72ad8)

- 运行结果：
    
    n = 2
    
    n = 3
    
    n = 4
    
- 案例1：打印问题。
- 案例2：计算阶乘。

案例演示：**[Recursion.java](https://github.com/dnx00/Notes_on_the_Course_of_Han_Shunping_Gradually_Learning_Java/blob/main/Chapter07_%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%BC%96%E7%A8%8B%5B%E5%9F%BA%E7%A1%80%E9%83%A8%E5%88%86%5D/0215-0218_%E9%80%92%E5%BD%92%E6%89%A7%E8%A1%8C%E6%9C%BA%E5%88%B6/Recursion.java)**

- 递归重要规则
1. 执行一个方法时，就创建一个新的受保护的独立空间（栈空间）。
2. 方法的局部变量是独立的，不会相互影响，比如n变量。
3. 如果方法中使用的是引用类型变量（比如数组、对象），就会共享该引用类型的数据.。
4. 递归必须向退出递归的条件逼近，否则就是无限递归，出现StackOverflowError。
5. 当一个方法执行完毕，或者遇到return时，就会返回，遵守谁调用就将结果返回给谁，同时当方法执行完毕或者返回时，该方法也就执行完毕。

运行结果：  
==案例1. 打印问题==  
n = 2  
n = 3  
n = 4  

==案例2. 计算阶乘==  
3! = 6  
