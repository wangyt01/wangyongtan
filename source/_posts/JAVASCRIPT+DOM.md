# 第一章  JavaScript简史  

## 本章内容  

# 第二章  JavaScript 语法  

## 本章内容  
1. 语句  
2. 变量和数组  
3. 操作符  
4. 条件语句和循环对象  
5. 函数和对象  

本章将对JavaScript语法中重要的概念进行简要的介绍。  

## 2.1 准备工作  
  编写JavaScript脚本不需要任何的软件，一个文本编辑器和一个Web浏览器就够了。  
  用JavaScript编写的代码必须嵌在一份HTML/XHTML文案中才能得以执行。这可以通过两种方法做到。第一种办法是将JavaScript代码插在文档<head>部分的<script>标签间，如下所示：
	<!DOCTYPE html>
	<html>
	<head>
	<script type="text/javascript">
	JavaScript goes here...
	</script>
	</head>
	</body>
	Mark-up goes here...
	</html>  

更好的办法是先把JavaScript代码存入一个独立的文件————建议把.js作为这种文件的扩展名，再利用<script>标签的src属性指向该文件，如下所示：
	<!DOCTYPE html>
	<html>
	<head>
	<script type="text/javascript" src="test.js">
	</script>
	</head>
	</body>
	Mark-up goes here...
	</html>    

如果

## 2.2 语法	

  英语中是一种解释型的语言。在阅读和处理别人用英文写出来的文字时，阅读者本人就相当于一个英语解释器。只要作者遵守了英语的语法规则，他想表达的意思就可以被阅读者正确地解读出来。语法(syntax)的广义含义包括语句、单词、标点符号等各个方面，它的狭义含义则特指语句结构方面的各项规则。在接下来的讨论中，我们使用的是“语法”这个词的狭义含义。  

与那些有文字的人类语言一样，每种程序设计语言都有自己的语法。JavaScript语言的语法与Java和C++等其他一些程序设计语言的语法非常相似。  

## 2.3 语句  

用JavaScript或任何一种其他程序设计语言编写出来的脚本都是由一系列指令构成的，这些指令称为语句(statement)。只有按照正确地语法编写出来的语句才能得到正确的解释。  

JavaScript语句与英语的句子很相似。它们是任何一个脚本的基本构成单位。  
英语语法要求每个句子必须以一个大写字母开头、以一个句号结尾。JavaScript在这方面的要求不那么严格，程序员只需简单地把各条语句放在不同的行上就可以分隔它们，如下所示：
	first statement
	second statement  

如果你想把多条语句放在同一行上，就必须像下面这样用分号来分隔它们：  
	first statement; second statement;  
即使么有把多条语句放在同一行上，但在每行语句的末尾加上一个分号，也是一种良好的编程习惯：  
	first statemtent;
	second statement;  

这可以让代码更容易阅读。将每条语句单独占用一行的做法可以让你本人或者其他程序员更容易追踪JavaScript脚本的执行流程。  
