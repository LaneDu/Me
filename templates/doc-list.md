.action{$docname:=.title}
.action{$docid:=.id}
.action{$block:= (queryBlocks "select * from blocks where type= 'd' and path like '%?%' and id !='?' " $docname $docid)}

## **.action{$docname}目录**{: style="background-image: linear-gradient(to right, var(--b3-theme-primary), var(--b3-theme-error)); -webkit-background-clip: text; color: transparent;"}

{: id="20210308150148-9b4w9s0" memo="新建文件夹名字的文档，然后调用该模板"}

.action{"| 序号 | 内容 | 路径 |"}
.action{"| ------ | ------ | ------ |"}
.action{range $index,$v:=$block}  | .action{add $index 1} | ((.action{$v.ID} ".action{$v.Content}")) | .action{$v.Path} |
.action{end}

注意：该文档要和文件夹同名
