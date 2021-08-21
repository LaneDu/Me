.action{$docid:=.id}
.action{$docname:=.title}
.action{$block := (queryBlocks "select * from blocks where type='d' and id ='?' "  $docid)}
.action{$filePath :=" "}
.action{$fileBox :=" "}
.action{$dirPath := " "}

.action{/*获取文件的目录路径*/}
	.action{range $index,$v:=$block}
		.action{$filePath = $v.HPath}
		.action{$fileBox =  $v.Box}
	.action{end}
	
.action{/*获取目录包括子目录下所有的文件*/}
	.action{$block := (queryBlocks "select * from blocks where hpath like'?/%' and type='d' and box='?' order by hpath asc limit 1000"  $filePath  $fileBox)}

.action{/*"输出双链"*/}
	.action{$b :=""}
	.action{range $v:=$block}
  .action{$c := $v.HPath | replace $filePath " " }
  .action{$c  = trimAll " / " $c}
	.action{$a := split "/" $c}
	.action{range $a1:=$a}
 	.action{$b =cat $b "-" " "}
	.action{end} 
.action{$b} ((.action{$v.ID}))
.action{$b =""}
.action{end}

