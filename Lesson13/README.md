Lambda表达式2
============

## 知识点

* 函数型接口(java.util.function)

## Lambda写法

~~~java
( 参数 ) -> { 处理 }
~~~

## 实战演习

~~~java
import java.util.function.BiFunction;
import java.util.function.Function;

public class Main {
    public static void main(String[] args) {
        /**
         * 函数型接口
         */
        // Function<T, R>
        // T:参数类型
        // R:返回值类型
        Function<Integer, Integer> multi2 = (i) -> {
            return i * 2;
        };
        System.out.println(multi2.apply(10));

        // BiFunction<T,U,R>
        // T:第1参数类型
        // U:第2参数类型
        // R:返回值类型
        BiFunction<Integer, Integer, Integer> addfunc = (a, b) -> {
            return a + b;
        };
        int result = addfunc.apply(10, 20);
        System.out.println(result);

        BiFunction<Integer, Integer, Integer> minusfunc = (a, b) -> {
            return a - b;
        };
        result = minusfunc.apply(10, 20);
        System.out.println(result);
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
