.action{$docid:=.id}
.action{$docname:=.title}
.action{$block := (queryBlocks "select * from blocks where type='d' and id ='?' "  $docid)}
.action{$filePath :=" "}
.action{$fileBox :=" "}
.action{$dirPath := " "}
.action{$numOfSearch := 0}

.action{$regexDirPath:="(/(\\.|\\w|\\s|-|[^x00-xff])+)*/"}

.action{/*获取文件的目录路径*/}
	.action{range $index,$v:=$block}
		.action{$filePath = $v.HPath}
		.action{$fileBox =  $v.Box}
	.action{end}
	.action{/*通过正则表达式获取该文件所在的文件夹*/}
	.action{$dirPath =(regexFind  $regexDirPath  $filePath )}
	
.action{/*获取目录包括子目录下所有的文件*/}
	.action{$block := (queryBlocks "select * from blocks where hpath like'?%' and type='d' and box='?' order by hpath asc limit 1000"  $dirPath $fileBox)}
	

.action{/*获取所有文件夹路径*/}
.action{$filePathList:= list $dirPath}
.action{range $index, $v:=$block}
	

	.action{$filePath = (regexFind  $regexDirPath  $v.HPath )}
	
	.action{if not (has  $filePath $filePathList)}
		.action{$filePathList = append  $filePathList $filePath}
	.action{end}	
	.action{$numOfSearch = $index}
.action{end}

.action{/*输出双链*/}
.action{range $listItem:=$filePathList}
.action{$title:=trimAll "/" $listItem}
.action{if contains "/" $title }
.action{$title =splitn "/" 3 $listItem}
.action{$title = $title._2}
.action{end}

##### .action{trimAll "/" $title}
	.action{range $v:=$block}
	
	.action{$filePath = (regexFind  $regexDirPath  $v.HPath )}
	
	.action{if eq $listItem $filePath }
- ((.action{$v.ID}))
	.action{end}
	
	.action{end}
	.action{end}

