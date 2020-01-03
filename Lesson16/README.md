StringBuffer和StringBuilder
==========================

## 知识点

* 字符串叠加处理
* String += String(效率低下)
* StringBuffer(线程安全)
* StringBuilder(速度优势)

## 实战演习

~~~java
public class Main {

    public static void main(String[] args) {
        /**
         * 字符串叠加(效率低下)
         */
        String content = "";
        content += "我学习Java";
        content += "我学习Android";
        content += "我学习JavaEE";
        System.out.println(content);

        /**
         * StringBuffer(线程安全)
         */
        StringBuffer stringBuffer = new StringBuffer();
        stringBuffer.append("我学习Java");
        stringBuffer.append("我学习Android");
        stringBuffer.append("我学习JavaEE");
        System.out.println(stringBuffer.toString());

        /**
         * StringBuilder(速度优势)
         */
        StringBuilder stringBuilder = new StringBuilder();
        stringBuilder.append("我学习Java");
        stringBuilder.append("我学习Android");
        stringBuilder.append("我学习JavaEE");
        System.out.println(stringBuilder.toString());
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
