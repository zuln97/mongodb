>>Create db
>use DB_Name

>>What is DB_name used?
>db

>>Show DB list
>show dbs

>>Delete DB
>db.dropDatabase()


------------Export & Import database--------------------
>>Binary
>Import database
mongorestore -h ds119734.mlab.com:19734 -d rfid -u <user> -p <password> <input db directory>

>Export database
mongodump -h ds119734.mlab.com:19734 -d rfid -u <user> -p <password> -o <output directory>

>Import collection
mongorestore -h ds119734.mlab.com:19734 -d rfid -u <user> -p <password> <input .bson file>

>Export collection
mongodump -h ds119734.mlab.com:19734 -d rfid -c <collection> -u <user> -p <password> -o <output directory>

>>JSON
>Import collection
mongoimport -h ds119734.mlab.com:19734 -d rfid -c <collection> -u <user> -p <password> --file <input file>

>Export collection
mongoexport -h ds119734.mlab.com:19734 -d rfid -c <collection> -u <user> -p <password> -o <output file>

>>CSV
>Import collection
mongoimport -h ds119734.mlab.com:19734 -d rfid -c <collection> -u <user> -p <password> --file <input .csv file> --type csv --headerline

>Export collection
mongoexport -h ds119734.mlab.com:19734 -d rfid -c <collection> -u <user> -p <password> -o <output .csv file> --csv -f <comma-separated list of field names>

-------------------------------------------------------

NodeJs and Mongoose
