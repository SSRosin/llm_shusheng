
# 一.Python 实现wordcount
    # import re
    from collections import defaultdict


    def wordcount(text):
    # 去掉标点符号并将所有单词转换成小写
    text = text.lower()
    text = re.sub(r'[^\w\s]', '', text)

    # 使用正则表达式来匹配单词
    words = re.findall(r'\b\w+\b', text)

    # 使用 defaultdict 来统计每个单词的出现次数
    word_count = defaultdict(int)

    for word in words:
        word_count[word] += 1

    return dict(word_count)
# 运行结果
![GitHub Logo](./images/python_result.png)

# 二.调试过程
# 1.首先设置断点，并开启调试
![GitHub Logo](./images/断点.png)
# 2.点击不同的功能按钮，实现不同的操作
    如单步执行我的代码，会一行一行执行
![GitHub Logo](./images/单步.png)
# 
