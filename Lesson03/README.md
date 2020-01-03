静态字段(static)
================

## 知识点

* 静态字段
* 静态方法

## 实战演习

### Player.java

~~~java
...
    //静态字段
    public static String VERSION = "1.0.0";
    //静态方法
    public static void showVersion() {
        System.out.println(Player.class.toString() + " : " + VERSION);
    }
...
~~~

### Main.java

~~~java
public class Main {
    public static void main(String[] args) {
        Player player = new Player("");
        player.showVersion();
        Player.showVersion();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
