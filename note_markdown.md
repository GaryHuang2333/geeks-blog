MarkDown 语法笔记 : 

# 标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

# 分割线
***
---
___
上面三种分割线

# 段落换行
第一行
第二行(换行失败)  
第三行(换行成功,段落的换行是末尾添加两个空格加回车)  
第四行(换行成功)

# 字体
我的*斜体文字*  
我的**粗体文字**  
我的~~删除线文字~~  
我的<u>下划线文字</u>

# 区块
> 区块
>> 子区块
>>> 子子区块
>>>> 区块嵌套

# 列表
## 有序列表
1. 有序列表1
2. 有序列表2
    1. 有序列表2.1
    2. 有序列表2.2
    1. 有序列表2.3(错误序号自动纠正)
        1. 有序列表2.3.1
        2. 有序列表2.3.2
    10. 有序列表2.4(错误序号自动纠正)

## 无序列表
- 无序列表1
    - 无序列表1.1
    - 无序列表1.2
        - 无序列表1.2.1
        - 无序列表1.2.2
            - 无序列表1.2.2.1
            - 无序列表1.2.2.2
        - 无序列表1.2.3
    - 无序列表1.3
- 无序列表2
- 无序列表3  

* 无序列表1
    * 无序列表1.1
    * 无序列表1.2
        * 无序列表1.2.1
        * 无序列表1.2.2
            * 无序列表1.2.2.1
            * 无序列表1.2.2.2
        * 无序列表1.2.3
    * 无序列表1.3
* 无序列表2  

## 混序列表
1. 混序列表1
    - 混序列表1.1
    - 混序列表1.2
        1. 混序列表1.2.1
        2. 混序列表1.2.2
    - 混序列表1.3
2. 混序列表2
3. 混序列表3

# 链接
## 超链接
1. ```[链接名称](链接地址)```  
eg : [百度](http://www.baidu.com)
2.  ```<链接地址>```  
eg: <http://baidu.com>

## 图片
```![属性文本](图片地址)```  
eg: ![头像](./pic_path)  

## 图片超链接
```[图片](链接地址)```  
eg: [![头像](./pic_path)](http://www.baidu.com)  

# 代码块
## 代码块1(4个空格 or 一个制表符tab)
    String[] array = {"java", "c"};
    List<String> list = Arrays.asList(array);
    //但该方法存在一定的弊端，返回的list是Arrays里面的一个静态内部类，该类并未实现add,remove方法，因此在使用时存在局限性

    public static <T> List<T> asList(T... a) {
    //  注意该ArrayList并非java.util.ArrayList
    //  java.util.Arrays.ArrayList.ArrayList<T>(T[])
        return new ArrayList<>(a);
    }

## 代码块2(```)
```
String[] array = {"java", "c"};
List<String> list = Arrays.asList(array);
//但该方法存在一定的弊端，返回的list是Arrays里面的一个静态内部类，该类并未实现add,remove方法，因此在使用时存在局限性

public static <T> List<T> asList(T... a) {
//  注意该ArrayList并非java.util.ArrayList
//  java.util.Arrays.ArrayList.ArrayList<T>(T[])
    return new ArrayList<>(a);
}
```

## 代码块3(``` + 指定语言)
```java
String[] array = {"java", "c"};
List<String> list = Arrays.asList(array);
//但该方法存在一定的弊端，返回的list是Arrays里面的一个静态内部类，该类并未实现add,remove方法，因此在使用时存在局限性

public static <T> List<T> asList(T... a) {
//  注意该ArrayList并非java.util.ArrayList
//  java.util.Arrays.ArrayList.ArrayList<T>(T[])
    return new ArrayList<>(a);
}
```

# 表格
```
|表头|表头|
|-----|----|
|单元格|单元格|
|单元格|单元格|
|单元格|单元格|
```
eg:  
|表头|表头|
|-----|-----|
|单元格|单元格|
|单元格|单元格|
|单元格|单元格|

```
|左对齐|右对齐|中间对齐|
|:-----|----:|:----:|
|单元格|单元格|单元格|
|单元格|单元格|单元格|
|单元格|单元格|单元格|
```
eg:  
|左对齐|右对齐|中间对齐|
|:-----|----:|:----:|
|左|右|中|
|左|右|中|
|左|右|中|
