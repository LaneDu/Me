.action{ $ppath := nospace (cat "https://cdn.jsdelivr.net/gh/lanedu/SiYuan@main/pic/pic" ((randInt 1 234) | toString) ".jpg")}

.action{$after := (div ((toDate "2006-01-02" "2021-11-05").Sub now).Hours 24)}

.action{$dayleft := (div ((toDate "2006-01-02" "2022-01-01").Sub now).Hours 24)}

.action{$week := add (mod (div ((toDate "2006-01-02" "2050-03-13").Sub now).Hours 24) 7) 1}

![image.png](.action{$ppath})


> 🕐 创建时间：.action{now | date "2006-01-02 15:04"} .action{last (slice (list "星期六" "星期五" "星期四" "星期三" "星期二" "星期一" "星期天") 0 $week )}

### 🍎 上午

​     

### 🍉 下午

​     

### 🍒 晚上

​      

{{{row
💡 

​     

}}}
{:  style="color: var(--b3-card-info-color);background-color: var(--b3-font-background9);"}

### 🍓 Picture