{{SELECT * FROM blocks WHERE (id in (select parent_id from blocks where content like '%.action{.title}%' and type !='l' ) and type='i') and root_id !='.action{.id}' order by created DESC}}
{: id="20210113192134-ghsdpep" memo="提示：content like '%这里改成你要查询的关键字%'"}
