# c2py
JS将中文转化为拼音首字母字符串的小插件

fork自Alfred-kai/C2Pin

修改了获取首字母函数(firstChar)：

1. 英文和数字原样输出

2. 小写转大写

# Installation #
 **Direct download**

Download the script here and include it (unless you are packaging scripts somehow else):

`<script src="/path/to/c2py/index.js"></script>`

**Package Managers**

c2py supports npm and Bower under the name  c2py

**Import the library**

`import c2py from 'c2py'`

# Basic Usage 



Transfer Chinese to Pinyin with first letter

`c2py.firstChar()`

Transfer Chinese to Pinyin with full letter

`c2py.fullChar()`


# Namespace conflicts

If there is any danger of a conflict with the namespace c2py, the noConflict method will allow you to define a new namespace and preserve the original one.

    // Assign the c2py api to a different variable and restore the original "window.c2py"
    var c2pyCopy = c2py.noConflict();
    c2py.firstChar();