---
layout: post
title: My First Java Lesson
date: 2016-11-10 20:17
comments: true
external-url:
categories: Study Notes
---

程序员学写代码的时候，第一个程序总是hello world，它就好像是一个标志，代表“我正式开始学习这门语言啦！”的意思。


Java的程序，全部圈在一个个的class里面，主函数也一样。程序的第二行代码 import java.util.Scanner ，就好像C++里面的引入头文件的那一行 #include &lt;iostream&gt; 一样，只要有输入就必须加上去。

	Scanner in = new Scanner(System.in);
	System.out.println(in.nextLine());

任何需要读用户输入的程序都需要第一行。


	package hello;
	
	import java.util.Scanner;
	
	public class Hello {
	
		public static void main(String[] args) {
			// TODO Auto-generated method stub
	//		System.out.println("hello");
			//println 是带回车的输出，有点类似于printf里面的\n，而print单独是不带回车的输出
	//		java的in也需要声明，很奇怪
			Scanner in = new Scanner(System.in);
	//		System.out.println("echo:" + in.nextLine());
			System.out.print("请输入票面金额：");
			int amount = in.nextInt();
	//		System.out.println(a+b);
			System.out.print("请输入商品价格：");
			int price = in.nextInt();
			System.out.println(amount + "-"+price+"="+ ( amount-price));
		}
	
	}



