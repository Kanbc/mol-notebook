1. Schema Content ของเว็บเก่าจะอยู่ภายใต้ Tag <table name="node">  
2. Schema Content ของเว็บใหม่(ที่ต้องการ) จะอยู่ภายใต้ <item>
3. แนวทางคือ ดึงข้อมูลจาก Content ของเว็บเก่า แต่ละ Content (<table name="node">) มาใส่ ของเว็บใหม่ (ใน <item>)
4. Mapping 
        - <column name="node_title"> => <title>
        - <column name="nid"> => <wp:post_id>
        - <column name="node_data_field_document_mail_field_export_date_value"> => <pubDate>Wed, 12 Dec 2018 15:20:59 +0000</pubDate> ต้องเป็น Format ตามนี้