 # 实战1：TODO Checker #
 
 ## 功能描述 ##
- 我们在编写代码时常常会在代码中留下一些临时代码，通过TODO等关键字标识，这些临时代码通常用于打桩等临时措施，最终版本需要将这些代码通通修复。因此我们需要检查代码中是否有未完成的代码。 
- 我们可以通过编写todo_checker.py脚本，实现在指定文件夹下的文件中查找指定关键字，并显示关键字所在位置，帮助我们找到临时代码，及时修复。
 
 ## 输入参数 ##
 + 格式： todo_checker.py [-d dir1 dir2] [-k key1 key2]
 + 说明： 
    + []为可选带参数
    + -d 表示要搜索的文件夹，可以同时指定多个，不指定则默认为当前路径(不需要处理子文件夹)
    + -k 表示要搜索的关键字，可以同时指定多个，不指定则默认为“TODO”
 
 ## 结果判定 ##
 - 如果找到文件中有匹配到关键字的内容，打印如下：
    - 文件名(行号)：原文内容
    - filename.sv(233): a++; // TODO : some_coments
 - 如果没有找到匹配文字内容，打印如下
    - Check OK.
 
 ## Step-by-step ##
 ### 1、完成usage和sumary ###
 需要掌握标准输出和条件判断
 输入输出是与程序交互的
 
 ### 2、完成option_parser ###
 需要掌握list的操作
 
 ### 3、完成file_checker ###
 需要掌握文件操作、字符串匹配
 
 ### 4、完成folder_checker ###
 掌握文件夹查看、遍历等操作
