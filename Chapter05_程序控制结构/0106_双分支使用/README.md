# 0106_双分支使用

- 基本语法：
    
    if(条件表达式){
    
    执行代码块 1;   (可以有多条语句;)
    
    }else{
    
    执行代码块 2;   (可以有多条语句;)
    
    }
    
- 说明：当条件表达式为ture 时，就会执行代码块1；如果为false，就执行代码块2。
- 特别说明：如果执行代码块中只有一条语句，则可以不用{ }，建议写上{ }。
- 案例：编写一个程序，可以输入人的年龄，如果该同志的年龄大于18岁，就输出“年龄大于18岁！”，否则输出“年龄小于或等于18岁！”。

案例演示：**[If02.java](https://github.com/dnx00/Notes_on_the_Course_of_Han_Shunping_Gradually_Learning_Java/blob/main/Chapter05_%E7%A8%8B%E5%BA%8F%E6%8E%A7%E5%88%B6%E7%BB%93%E6%9E%84/0106_%E5%8F%8C%E5%88%86%E6%94%AF%E4%BD%BF%E7%94%A8/If02.java)**

运行结果1：  
请输入年龄：  
3  
年龄小于或等于18岁！  
程序继续向下运行：）  

运行结果2：  
请输入年龄：  
20  
年龄大于18岁！  
程序继续向下运行：）  
