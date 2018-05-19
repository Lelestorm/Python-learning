# [re](https://docs.python.org/3/library/re.html) - Regular expression operations

Source code: [Lib/re.py](https://github.com/python/cpython/tree/3.6/Lib/re.py)


### 特殊字符：
 `.`  默认模式下，匹配除换行符(\n - newline)外的任意字符。当指定[re.DOTALL](https://docs.python.org/3/library/re.html#re.DOTALL)标识时，匹配任意字符。
 
 `^`  \n 匹配字符串开始，MULTILINE（多行模式）下在每个换行符之后立即匹配。
 
 `$`  \n 匹配字符串结束或字符串结尾的换行符，并且在MULTILINE模式下也与换行符匹配。
 
 `*`  \n re* 匹配0多个（re）表达式。
 
 `+`  \n re+ 匹配1次或多次（re）表达式
 
 `?`  \n re? 匹配0或1次（re）表达式。
 
 `*?`, `+?`, `??` \n `*` `+` `?` 限定符都是贪婪的，他们匹配尽可能多的文本。有时这种行为是不需要的；如 `RE <.*>` 匹配 `'<a>b<c>'`, 他将匹配整个字符串，而不只是`'<a>'`。加上 `?` 限定符后将以非贪婪或最小的方式执行匹配; 尽可能少的字符被匹配。 RE `<.*?>` 只匹配 `'<a>'`。
