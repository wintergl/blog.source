title: 参考代码-java-StringUtils
date: 2015-11-4 20:00:29
tags: [code, java]
categories: 参考
toc: true
layout: no_side_bar
---
参考commons-lang包中的StringUtils, 可以对我们日常的开发工作有所帮助
<!-- more -->
### 空字符串检查
```java
StringUtils.isBlank(testString)
```
### 清除空白字符
```java
String test1 = "\t";
String test2 = "  A  Test  ";
String test3 = null;

//test1 trimToNull: null
System.out.println( "test1 trimToNull: " + StringUtils.trimToNull( test1 ) );
//test2 trimToNull: A  Test
System.out.println( "test2 trimToNull: " + StringUtils.trimToNull( test2 ) );
//test3 trimToNull: null
System.out.println( "test3 trimToNull: " + StringUtils.trimToNull( test3 ) );
```
### 取得字符串的缩写
```java
String test = "This is a test of the abbreviation.";
String test2 = "Test";

//This is a te...
System.out.println( StringUtils.abbreviate( test, 15 ) );
//...is a test...
System.out.println( StringUtils.abbreviate( test, 5,15 ) );
//Test
System.out.println( StringUtils.abbreviate( test2, 10 ) );
```
