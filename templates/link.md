## đˇ **éžćĽâ .action{.title}âçĺĺŽš**

{{SELECT * FROM blocks WHERE markdown LIKE '%.action{.id}%' and root_id != '.action{.id}'}}
## đˇ **ćĺâ .action{.title}âçĺĺŽš**

.action{/* SELECT * FROM blocks WHERE content LIKE '%.action{.title}%' and root_id != '.action{.id}' and markdown not LIKE '%.action{.id}%' */}

{{SELECT * FROM blocks WHERE (type='i' and id in (SELECT parent_id FROM blocks WHERE type='p' and (content LIKE '%.action{.title}%' or name LIKE '%.action{.title}%' or alias LIKE '%.action{.title}%' or ('.action{.alias}' !='' and content LIKE '%.action{.alias}%') or ('.action{.alias}' !='' and name LIKE '%.action{.alias}%') or ('.action{.alias}' !='' and alias LIKE '%.action{.alias}%'))) and markdown not LIKE '%.action{.id}%') or ( type !='l' and type != 'i' and  (content LIKE '%.action{.title}%' or name LIKE '%.action{.title}%' or alias LIKE '%.action{.title}%' or ('.action{.alias}' !='' and content LIKE '%.action{.alias}%') or ('.action{.alias}' !='' and name LIKE '%.action{.alias}%') or ('.action{.alias}' !='' and alias LIKE '%.action{.alias}%'))  and markdown not LIKE '%.action{.id}%' )and root_id !='.action{.id}' order by created DESC}}
