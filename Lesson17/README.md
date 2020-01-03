定时处理
=======

## 知识点

* Timer
* TimerTask

## 实战演习

~~~java
import java.text.SimpleDateFormat;
import java.util.Date;
import java.util.Timer;
import java.util.TimerTask;

public class Main {

    public static void main(String[] args) {

        SimpleDateFormat format = new SimpleDateFormat("[HH:mm:ss]");

        class MyTimerTask extends TimerTask {
            @Override
            public void run() {
                System.out.println(format.format(new Date()) + "MyTimerTask.run()...");
            }
        }

        Timer timer = new Timer();
        timer.schedule(new MyTimerTask(), 1000, 3000);
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
