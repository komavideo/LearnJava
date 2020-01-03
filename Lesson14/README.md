Lambda表达式3
============

## 知识点

* HashMap的使用

## Lambda写法

~~~java
( 参数 ) -> { 处理 }
~~~

## 实战演习

~~~java
import java.util.HashMap;
import java.util.Map;

public class Main {

    public static void main(String[] args) {
        Map<String, String> stringMap = new HashMap<>();
        stringMap.put("usa", "美国");
        stringMap.put("chn", "中国");
        stringMap.put("jpn", "日本");

        // 普通写法
        for (Map.Entry<String, String> item : stringMap.entrySet()) {
            System.out.println("●" + item.getKey() + ":" + item.getValue());
        }

        // Lambda式写法
        stringMap.forEach((key, value) -> {
            System.out.println("■" + key + ":" + value);
        });
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
