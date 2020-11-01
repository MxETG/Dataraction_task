# dataraction_task
## DB design (NoSQL partitioned)
Document DB1: order_info, partitioned by order_time \
order_id: unique \
session_id, table_id: index \
order_time, finish_time \
total_price \
order_items: JSON array of (item_id, item_quantity) \
status: Not_finished(0), finished(1), cancel \

Document DB2: item_info \
item_id: unique, index \
item_price \
item_name \
item_description \
item_category \
item_image: url
