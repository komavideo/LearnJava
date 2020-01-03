包管理(package)
===============

Java的包管理主要用于把众多的类文件进行分类，便于分别管理和维护。

## 知识点

* 包定义
* package pkg1[．pkg2[．pkg3…]];

包其实就是文件夹，包定义只要遵循文件夹的结构就可以执行。

## 实战演习

### MyUtil.java

~~~java
package com.komavideo.util;

public class MyUtil {
    public static int add(int x, int y) {
        return x + y;
    }
}
~~~

### Player.java

~~~java
package com.komavideo.entity;

public class Player {
    private String name;

    public Player(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public void sayHelo() {
        System.out.println("Helo " + this.name + ".");
    }
}
~~~

### Main.java

~~~java
package com.komavideo;

import com.komavideo.entity.Player;
import com.komavideo.util.MyUtil;

public class Main {
    public static void main(String[] args) {
        int result = MyUtil.add(10, 20);
        System.out.println("result=" + result);

        Player player = new Player("Koma");
        player.sayHelo();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
