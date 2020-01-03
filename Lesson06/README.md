集合与泛型
=========

## 知识点

* List<>
* ArrayList<>

集合与数组类似的数据结构，但集合更容易操作，也支持更多的算法。

泛型可以让集合更加高效，支持更多的数据类型。

## 实战演习

### Main.java

~~~java
import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        List<String> list1 = new ArrayList<String>();
        List<String> list2 = new ArrayList<>();
        runS(list1);

        List<Integer> list3 = new ArrayList<>();
        runI(list3);
    }

    private static void runS(List<String> list) {
        list.add("Curry");
        list.add("Harden");
        list.add("LeBron");

        for (String player : list) {
            System.out.println(player);
        }
    }

    private static void runI(List<Integer> list) {
        list.add(100);
        list.add(200);
        list.add(300);

        for (int num : list) {
            System.out.println(num);
        }
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
