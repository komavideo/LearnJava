匿名类
======

## 知识点

* 线上类
* 匿名类

## 实战演习

### Main.java

~~~java
//数据库接口
interface IDatabase {
    void connect(String connString);
    void close();
}

public class Main {

    public static void main(String[] args) {

        /**
         * 线上Oracle类
         */
        class Oracle implements IDatabase {
            @Override
            public void connect(String connString) {
                System.out.println("连接Oracle");
            }

            @Override
            public void close() {
                System.out.println("关闭Oracle");
            }
        }
        IDatabase oracle = new Oracle();
        oracle.connect("ip/uid/pwd");
        oracle.close();

        /**
         * 匿名类
         */
        IDatabase mysql = new IDatabase() {
            @Override
            public void connect(String connString) {
                System.out.println("连接MySQL");
            }

            @Override
            public void close() {
                System.out.println("关闭MySQL");
            }
        };
        mysql.connect("ip/uid/pwd");
        mysql.close();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
