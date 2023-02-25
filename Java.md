# Java

## 一.Java EE

### 1.Java基础

#### (1) 常见cmd命令



![wps1](./images/wps1-1677297845562-1.jpg)

#### (2) 一个基础Java代码

```java
public class hello {
	public static void main(String[] args) {
		System.out.println("hello world");
	}

}
```

#### (3) 字符类型![wps3](./images/wps3.jpg)

/t 制表符的使用：补全前八个位置的空格![wps4](./images/wps4.jpg)

#### (4) 基本数据类型![wps5](./images/wps5.jpg)

#### (5) 键盘录入介绍![wps6](./images/wps6.jpg)

#### (6) Java结构介绍![wps7](./images/wps7.jpg)

#### (7) 随机数生成器 ![wps8](./images/wps8.jpg)![wps9](./images/wps9.jpg)

```java
猜数小游戏
package com.heima4;

import java.util.Random;
import java.util.Scanner;

public class FourDemo2 {
    public static void main(String[] args) {
        Random r=new Random();
        int number=r.nextInt(10)+1;
        Scanner input=new Scanner(System.in);
        System.out.println("请输入数字");

        for(int i=5;i>0;i--){
            int GuessNumber=input.nextInt();
            if(GuessNumber>number)
                System.out.println("猜大了，请再来一次,您还有"+(i-1)+"次机会");
            else if(GuessNumber<number)
                System.out.println("猜小了，请再来一次,您还有"+(i-1)+"次机会");
            else {
                System.out.println("恭喜您！猜对了！");
           break; }
        }


    }
}
```

#### (8) 方法的调用

1：我要干嘛？

2：我干这件事情需要什么才能完成？

3：调用处是否需要继续使用方法结果？

1. 无参方法![wps10](./images/wps10.jpg)

2. 有参方法![wps11](./images/wps11.jpg)

3. 有返回值的方法![wps12](./images/wps12.jpg)

   方法的重载：在同一个类中，方法名相同，参数不同的方法。与返回值无关。

### 2.Java 面向对象

   创建一个对象，调用对象，类似于C++里面的结构体

   注意创建的类里面没有static关键字，因为它不是静态的

   #### ![wps13](./images/wps13.jpg)

   #### (1) 封装的使用

![wps14](./images/wps14.jpg)

#### (2) private关键字

![wps15](./images/wps15.jpg)

数据调用

![wps16](./images/wps16.jpg)

![wps17](./images/wps17.jpg)

#### (3) this关键字

区分成员变量和局部变量

this关键字调用成员变量，否则就近原则

this的本质：代表方法调用者的地址值s.age==this.age

<img src="C:\Users\32414\AppData\Roaming\Typora\typora-user-images\image-20230225001521831.png" alt="image-20230225001521831" style="zoom:50%;" />

#### (4) Javabean

1. 构造方法![wps18](./images/wps18.jpg)
2. 调用方法![wps19](./images/wps19.jpg)
3. ![wps20](./images/wps20.jpg)
4. 标准的JavaBean![wps21](./images/wps21.jpg)

#### (5) 局部变量和成员变量

![wps22](./images/wps22.jpg)

#### (6) 占位符%s



![wps23](./images/wps23.jpg)

#### (7) 键盘录入大全

![wps24](./images/wps24.jpg)

#### (8) 字符串定义

![wps25](./images/wps25.jpg)

![wps26](./images/wps26.jpg)

#### (9) 字符串比较值的判断

“==”：

基本数据类型比较的是数据值

引用数据类型比较的是地址值![wps27](./images/wps27.jpg)

![wps28](./images/wps28.jpg)

#### (10) 遍历字符串

![wps29](./images/wps29.jpg)![wps30](./C:/Users/32414/Desktop/images/wps30.jpg)

#### (11) 截取方法substring(左，右)

![微信图片_20230225121322](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225121322.png)![wps31](./images/wps31.jpg)

#### (12) 替换方法replace(旧值，新值)

![wps32](./images/wps32.jpg)![wps33](./images/wps33-1677298482752-34.jpg)

#### (13) StringBuilder用法

![wps34](./images/wps34.jpg)

![wps35](./images/wps35.jpg)![wps36](./images/wps36.jpg)

![wps37](./images/wps37.jpg)

![wps38](./images/wps38.jpg)

![wps39](./images/wps39.jpg)

#### (14) 链式编程方法![wps40](./images/wps40.jpg)

#### (15) StringJoiner用法

![wps41](./images/wps41.jpg)

![wps42](./images/wps42.jpg)

![wps43](./images/wps43.jpg)



#### (16) 字符串转字符数组

![wps44](./images/wps44.jpg)

#### (17) 字符数组转字符串

![wps45](./images/wps45.jpg)

#### (18) 集合

![wps46](./images/wps46.jpg)

![wps47](./images/wps47.jpg)

![wps48](./images/wps48.jpg)![wps49](./images/wps49.jpg)

![wps50](./images/wps50.jpg)

上面str记录的是被删除的元素

![wps51](./images/wps51.jpg)

上面result记录的是被修改的元素，修改后的元素在list里面

![wps52](./images/wps52.jpg)

![wps53](./images/wps53.jpg)

键盘录入学生信息并存入集合

注意集合开始长度为0，用数字3替代循环次数

![wps54](./images/wps54.jpg)

集合作为返回值调用的方法

![wps55](./images/wps55.jpg)

![wps56](./images/wps56.jpg)

![wps57](./images/wps57.jpg)

#### (19) while退出多重循环

![wps58](./images/wps58.jpg)

#### (20) static关键字

一次调用永久使用(共享)

![wps59](./images/wps59.jpg)



![wps60](./images/wps60.png)

![wps63](./images/wps63.jpg)![wps64](./images/wps64.jpg)



#### (21) 工具类

![wps61](./images/wps61.jpg)

调用

![wps62](./images/wps62.jpg)

#### (22) 继承

![wps65](./images/wps65.jpg)

![wps66](./images/wps66.jpg)

##### ① 子类不能访问父类private类

![wps67](./images/wps67.jpg)

![wps68](./images/wps68.jpg)

##### ② 构造方法不能被继承

![wps69](./images/wps69.jpg)

成员变量可以被继承

非私有直接继承

private用set/get()方法继承



非私有成员方法可以继承

private成员方法不能被继承

![wps70](./images/wps70.jpg)

#####    ③ 成员变量继承语法![wps71](./images/wps71.jpg)

![wps72](./images/wps72.jpg)

##### ④ 成员方法继承语法

(this可以省略)

![wps73](./images/wps73.jpg)

##### ⑤ 方法重写

![wps74](./images/wps74.jpg)

![wps75](./images/wps75.jpg)

![wps76](./images/wps76.jpg)

#####    ⑥ 构造方法的访问

![wps77](./images/wps77.jpg)

##### ⑦ 带参方法构造的调用

![wps78](./images/wps78.jpg)

<img src="C:\Users\32414\AppData\Roaming\Typora\typora-user-images\image-20230225004638745.png" alt="image-20230225004638745" style="zoom:80%;" />

this(…)一般用处是设置默认值

![wps79](./images/wps79.jpg)

#### (23) 多态

![wps80](./images/wps80.jpg)

多态调用

变量是左边，方法是右边

![wps81](./images/wps81.jpg)

![wps82](./images/wps82.jpg)

##### 	① 多态的优势与弊端

![微信图片_20230225122523](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225122523.png)

![wps83](./images/wps83.jpg)

编译看左边，没有子类方法就会报错，不能使用子类的特有功能，只能将父类强转换为子类才能使用子类的特有功能

![wps84](./images/wps84.jpg)

##### ② instanceof关键字

判断a是不是狗类型，是返回true，否则false

![wps85](./images/wps85.jpg)

#### (24) 包

![wps86](./images/wps86.jpg)

#### (25) final关键字

<img src="C:\Users\32414\AppData\Roaming\Typora\typora-user-images\image-20230225005002498.png" alt="image-20230225005002498" style="zoom:67%;" />

final修饰常量![wps87](./images/wps87.jpg)

![wps88](./images/wps88.jpg)

#### (25) 权限修饰符

![微信图片_20230225122748](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225122748.png)



#### (26) 静态代码块

![微信图片_20230225122908](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225122908.png)

#### (27) 抽象类

关键字 abstract

作用：强制统一方法类型

![微信图片_20230225122946](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225122946.png)

![微信图片_20230225123028](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123028.png)

不能实例化意思是不能被创建对象

![微信图片_20230225123112](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123112.png)

#### (28) 接口

关键字interface定义

![微信图片_20230225123143](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123143.png)

关键字implements调用

![微信图片_20230225123240](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123240.png)



![微信图片_20230225123410](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123410.png)



![微信图片_20230225123454](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123454.png)

#### (29) default关键字

![微信图片_20230225123527](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123527.png)



接口中的静态方法

只能被接口调用，不能被重写

![微信图片_20230225123555](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123555.png)

#### (30) 内部类

成员内部类

![微信图片_20230225123636](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123636.png)



![微信图片_20230225123710](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123710.png)



##### ① 静态内部类

![微信图片_20230225123742](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123742.png)

##### ② 局部内部类

![微信图片_20230225123807](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123807.png)

##### ③ 匿名内部类

![微信图片_20230225123852](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225123852.png)



分号前面看作一个对象



![微信图片_20230225115533](./images/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20230225115533.jpg)