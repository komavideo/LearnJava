循环处理
=======

## 知识点

* while
* do-while
* for(...)

## 实战演习

~~~java
public class Main {

    public static void main(String[] args) {
        /**
         * 1:while循环
         */
        int count = 5;
        while (count > 0) {
            System.out.println("1:count:" + count);
            count--;
        }

        /**
         * 2:do-while循环
         */
        count = 5;
        do {
            System.out.println("2:count:" + count);
            count--;
        } while (count > 0);


        /**
         * 3:for循环
         */
        for (int i = 0; i <= 5; i++) {
            System.out.println("3:i:" + i);
        }
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
