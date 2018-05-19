# [re](https://docs.python.org/3/library/re.html) - Regular expression operations

Source code: [Lib/re.py](https://github.com/python/cpython/tree/3.6/Lib/re.py)


### 特殊字符：
 `.`  默认模式下，匹配除换行符(\n - newline)外的任意字符。当指定re.DOTALL标识时，匹配任意字符。
 
 `^`  匹配字符串的开始，MULTILINE（多行模式）下在每个换行符之后立即匹配。
