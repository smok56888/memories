# memories
回忆录，随手记一些好玩的小技巧。

## linux

### 批量备份不同文件夹下的同名文件到各自文件夹
<code>find /指定目录 -name '指定文件名' |awk '{cmd="cp "$1" "$1".bak20171025";system(cmd)}'</code>

### 批量替换不同文件夹下的同名文件里的字符串
<code>sed -i "s/需要替换的文本/新文本/g"  `find /指定目录 -name "指定文件名" `</code>
