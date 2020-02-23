# Cool Dashboard Plug-in

![Screenshot](https://raw.githubusercontent.com/sattuvirus/cool_dashboard_plugin/master/screenshot.gif)

This is a Region Dashboard Plug-in for Oracle APEX that let's you easily create some nice, responsive Cool Dashboard Design Cards. These Cards can be shown in a small Information with your application details with an icon and hover effects also added.

In this Dashboard plugin , Below 12 color classes that you can use in your sql query.
```
.db2_trendy_pink ,
.db2_tropical_blue ,
.db2_inter_orange 
.db2_azalea ,
.db2_dark_red ,
.db2_red,
.db2_blue,
.db2_green,
.db2_orange,
.db2_pink,
.db2_gossip,
.db2_tara
```

When you use these Dashboard plugin in Apex, below sql query will help to create sample Dashboard.
```
Select 1 as sort_order,
'All Data' title,
 '1' DATA1,
'fa fa-check-square-o ' as icon_class,
'db2_red' as container_class,
 apex_page.get_url(
    p_page        => 2,
    p_clear_cache => 2,
    p_items       => 'P4_USER_ID',
    p_values      => '1') as text
from Dual 
 union all
Select 2 as sort_order,
'Confirmed ' title,
 '2' data1,
  'fa fa-comments'   as  icon_class
     , 'db2_blue'     as  container_class,
     apex_page.get_url(
    p_page        => 2,
    p_clear_cache => 2,
    p_items       => 'P4_USER_ID',
    p_values      => '1') as text
from Dual 
    union all
   Select 3 as sort_order,
'Pending' title,
 '3' data1,
  'fa fa-cubes'   as  icon_class
     , 'db2_green'     as  container_class,
     apex_page.get_url(
    p_page        => 2,
    p_clear_cache => 2,
    p_items       => 'P4_USER_ID',
    p_values      => '1') as text
from Dual 
 union all
   Select 4 as sort_order,
'Cancel' title,
 '4' data1,
  'fa fa-tint'   as  icon_class
     , 'db2_orange'     as  container_class,
    apex_page.get_url(
    p_page        => 2,
    p_clear_cache => 2,
    p_items       => 'P4_USER_ID',
    p_values      => '1') as text
from Dual 
order by 1
```	
For working Demo just click on:
<a href ="https://apex.oracle.com/pls/apex/f?p=140847:3"> <h4>Demo</h4></a>

If you like my stuff, Please Like share and comment.
