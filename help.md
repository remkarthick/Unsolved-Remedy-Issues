# Query to get the Packing List Name based on the Webservice name

select name as packinglistname from arcontainer where containerid in (
select containerid from arreference where referenceobjid in (select containerid from arcontainer where name='<Type your webservice name here>' and containertype=5)
)
