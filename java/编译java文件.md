##编译Java文件##
**一、jad工具查看java 文件的字节码反编译成java文件**

- （1）编译Test.java文件得到.class文件: javac Test.java
- （2）执行： java Test 
- （3）下载jad 
- http://www.javadecompilers.com/jad
- **(4)jad 命令**
- (4.1)jad Test.class
- (4.2)会生成 Test.jad文件
- (4.3)然后执行 jad -sjava Test.clas

**二、javap 查看Java字节码**

- javac Test.java
- javap Test.class
- javap -c Test.class
 