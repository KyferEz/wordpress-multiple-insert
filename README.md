# Wordpress Multiple Insert
A Wordpress method for inserting multiple rows in a safer and faster way

# usage example
```
       $insert_arrays = array();
       foreach($assets as $asset) {
	   $time = current_time( 'mysql' );
       $insert_arrays[0] = array(
       'type' => "multiple_row_insert",
       'status' => 1,
       'name'=>"gordon freeman",
       'added_date' => $time,
       'last_update' => $time);
       $insert_arrays[1] = array(
       'type' => "multiple_row_insert",
       'status' => 2,
       'name'=>"captain dance",
       'added_date' => $time,
       'last_update' => $time);
       $insert_arrays[2] = array(
       'type' => "multiple_row_insert",
       'status' => 3,
       'name'=>"doc. emmet l. brown",
       'added_date' => $time,
       'last_update' => $time);
	   
       }
     
       wp_insert_rows($insert_arrays);
 ```
 
 
 source : http://stackoverflow.com/a/12374838/1194797
