# mywiser
倒排索引建立过程
----
**1.通过解析 https://dumps.wikimedia.org/zhwiki/latest/zhwiki-latest-pages-articles.xml.bz2的超大XML文件**


**2.将解析到的XML title和body进行ngram分词存入到postlist_value和postlist里面；产生了一个临时的buffer hash**

**3.轮训2步骤；对内存中的buffer hash进行合并**

**4.当内存或者存储达到一定条件后将buffer hash和存入在db中的hash进行合并**

**5.完成倒排索引的建立过程**



搜索过程
----
**待续**
