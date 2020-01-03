Lambda表达式1
============

## 知识点

* 什么是Lambda表达式？

Lambda式是一种匿名的嵌入类或函数，或者叫做闭包，它不需要做实际的类（或函数）的声明，却可以将具体的操作处理嵌入到代码当中。

* 优点：代码更加简洁
* 缺点：代码可读性变差

**天书解释**

Lambda式实质是某种规律的抽象实现。(>_<)

## Lambda写法

~~~java
( 参数 ) -> { 处理 }
~~~

## 实战演习

~~~java
/**
 * 单方法无参数接口
 */
interface IDatabase {
    void update();
}

public class Main {
    public static void main(String[] args) {
        // 接口
        IDatabase userDB = new IDatabase() {
            @Override
            public void update() {
                System.out.println(">>>数据库更新完成<<<");
            }
        };
        userDB.update();

        // Lambda式
        IDatabase blogDB = () -> {
            System.out.println("---更新博客数据库---");
        };
        blogDB.update();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
