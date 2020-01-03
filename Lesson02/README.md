Java的类
========

## 知识点

* 一切都是对象Class

在Java的世界里，一切都是对象间的操作，对象实例彼此协作，共同完成程序的功能。

## 实战演习

### Player.java

~~~java
//包定义
package com.komavideo;
//类定义
public class Player {
    //内部属性
    private String name;

    //构造器
    public Player(String name) {
        this.name = name;
    }

    //标准类方法
    public void shootBall2() {
        System.out.println(this.name + " 2分投球！");
    }

    //getter
    public String getName() {
        return name;
    }

    //setter
    public void setName(String name) {
        this.name = name;
    }
}
~~~

### Main.java

~~~java
package com.komavideo;
public class Main {
    //程序入库函数
    public static void main(String[] args) {
        System.out.println("Helo Java World!");
        Player player = new Player("库里");
        player.shootBall2();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
