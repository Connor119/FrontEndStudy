# JS Study

JS(世界上最流行的脚本语言)

### 基本使用

引入方式（内部或者外部）

```
<!--   方式2（外部引入）：使用src标签将脚本引入进来-->
    <script src="js/first.js"></script>

<!--  方式1（内部标签）：在这里直接写出js-->
    <script>

    </script>
```

### 语法入门

##### 定义变量：一切变量都叫做var（全局），局部变量就是（let）

```js

var variable1 = 1;
var variable2 = "2";

```

##### 条件控制(同java)，js是严格区分大小写的

```js
if(2>1){
    if(true){
        if(true){

        }
    }
    alert('true');
}
```



##### debug

在控制台中的sources中打断电使用

<img src="C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20220509173728767.png" alt="image-20220509173728767" style="zoom:50%;" />

蓝箭头是打断点，红箭头是步进



##### 控制台的**Application**

相当于web中的数据库

<img src="C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20220509174048112.png" alt="image-20220509174048112" style="zoom:50%;" />



##### js数据类型

**number**：不区分小数和整数与java不同

其中详细包括

<img src="C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20220509174735776.png" alt="image-20220509174735776" style="zoom: 50%;" />



**字符串**

单引号双引号都可以

**布尔值**

同java



**比较运算**（不太一样有三个等于号的比较）

这里一定要注意类型意义值也意义需要使用**三个等于号**

![image-20220509175140450](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20220509175140450.png)

坚持不使用==进行比较

- NaN===NaN是false
- 只能通过isNaN进行判断是否是NaN

浮点数问题（尽量避免使用浮点数进行比较运算）

![image-20220509175709348](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20220509175709348.png)

以上代码运行出来时false（精度损失）



**null和undefined**（java没有）

null是空

undefined未定义：对一个没有定义过的变量进行操作



**数组**

java是一些列相同类型的对象，js不用相同的类型

直接使用一个中括号即可

```
var arr =[1,2,3,'dff'];
```

用中括号取值

```
arr[0]
```

取数组下标如果越界了就是一个undefined



**对象**

java中必须有**类**之后才能new对象，js则不然**对象是用大括号括起来**

java中的匿名内部类（必须在接口上，在抽象类上实现）

```java
abstract class Person {
    public abstract void eat();
}
 
public class Demo {
    public static void main(String[] args) {
        Person p = new Person() {
            public void eat() {
                System.out.println("eat something");
            }
        };
        p.eat();
    }
}
```

js中的对象

```
var person = {
	在这里写成员属性和方法
}
```

每个属性之间通过逗号隔开，最后一个不需要

















