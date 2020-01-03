类继承
======

## 知识点

* extends:子类继承父类功能

## 实战演习

### Car.java

~~~java
public class Car {
    private int displacement;
    public Car(int displacement) {
        this.displacement = displacement;
    }
    public void showDisplacement() {
        System.out.println(this.getClass().toString() + " 排气量：" + this.displacement + "cc");
    }
}
~~~

### Bus.java

~~~java
public class Bus extends Car {
    public Bus(int displacement) {
        super(displacement);
    }
}
~~~

### Main.java

~~~java
public class Main {
    public static void main(String[] args) {
        Car car = new Car(2000);
        car.showDisplacement();
        Bus bus = new Bus(5000);
        bus.showDisplacement();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
