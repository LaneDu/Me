.action{/*来源 https://ld246.com/article/1629528735213 */}

.action{$docid:=.id}
.action{$block:= (queryBlocks "SELECT * FROM blocks WHERE type= 'd' AND path like '%/?/______________-_______.sy' Order BY hpath" $docid )}
.action{range $v:=$block} 

- ((.action{$v.ID} ".action{$v.Content}")) 


    .action{$block:= (queryBlocks "SELECT * FROM blocks WHERE type= 'd' AND path like '%/?/______________-_______.sy' Order BY hpath" $v.ID)}
    .action{range $v:=$block}
    - ((.action{$v.ID} ".action{$v.Content}")) 
      .action{$block:= (queryBlocks "SELECT * FROM blocks WHERE type= 'd' AND path like '%/?/______________-_______.sy' Order BY hpath" $v.ID)}
      .action{range $v:=$block}
      - ((.action{$v.ID} ".action{$v.Content}"))   
        .action{$block:= (queryBlocks "SELECT * FROM blocks WHERE type= 'd' AND path like '%/?/______________-_______.sy' Order BY hpath" $v.ID)}
        .action{range $v:=$block}
        - ((.action{$v.ID} ".action{$v.Content}")) 
            .action{$block:= (queryBlocks "SELECT * FROM blocks WHERE type= 'd' AND path like '%/?/______________-_______.sy' Order BY hpath" $v.ID)}
            .action{range $v:=$block}
            - ((.action{$v.ID} ".action{$v.Content}"))   
                .action{$block:= (queryBlocks "SELECT * FROM blocks WHERE type= 'd' AND path like '%/?/______________-_______.sy' Order BY hpath" $v.ID)}
                .action{range $v:=$block}
                - ((.action{$v.ID} ".action{$v.Content}"))   
    
                .action{end}
            .action{end}
        .action{end}
    
     .action{end}        
    
    .action{end}

.action{end}

