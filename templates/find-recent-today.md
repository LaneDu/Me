## .action{ now | date "2006-01-02  Mon "} 今天更新的文档

.action{$from := now | date "20060102"}
.action{$to := (now | date_modify "+24h")| date "20060102"}

.action{$blocks :=queryBlocks "SELECT * FROM blocks WHERE id in (SELECT root_id FROM blocks WHERE (updated >= '?' AND updated <= '?' AND root_id != '?')) order by updated DESC Limit 10000" $from $to .id}

.action{range $b := $blocks}
📙 ((.action{$b.RootID} ".action{ trimPrefix "/" $b.HPath}"))
.action{end}

