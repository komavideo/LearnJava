接口与实现
=========

## 知识点

* 接口定义抽象逻辑

## 实战演习

### IDatabase.java

~~~java
public interface IDatabase {
    void connect();
    void close();
}
~~~

### Oracle.java

~~~java
public class Oracle implements IDatabase {
    @Override
    public void connect() {
        System.out.println(this.getClass().toString() + " 连接...");
    }
    @Override
    public void close() {
        System.out.println(this.getClass().toString() + " 关闭");
    }
}
~~~

### MySQL.java

~~~java
public class MySQL implements IDatabase {
    @Override
    public void connect() {
        System.out.println(this.getClass().toString() + " 连接...");
    }
    @Override
    public void close() {
        System.out.println(this.getClass().toString() + " 关闭");
    }
}
~~~

### Main.java

~~~java
public class Main {
    public static void main(String[] args) {
        System.out.println("-----Oracle-----");
        run(new Oracle());
        System.out.println("-----MySQL-----");
        run(new MySQL());
    }
    private static void run(IDatabase db){
        db.connect();
        db.close();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
