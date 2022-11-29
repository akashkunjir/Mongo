mongoimport --db test --collection student --file ""


Windows PowerShell
Copyright (C) 2014 Microsoft Corporation. All rights reserved.

PS C:\Users\admin> mongoimport --db test --collection movie --file "C:\DBT\MongoDB\MongoDB\movie.json"
2022-11-24T23:25:55.232+0530    connected to: mongodb://localhost/
2022-11-24T23:25:55.384+0530    18 document(s) imported successfully. 0 document(s) failed to import.
PS C:\Users\admin> mongo
MongoDB shell version v4.2.18-rc0
connecting to: mongodb://127.0.0.1:27017/?compressors=disabled&gssapiServiceName=mongodb
Implicit session: session { "id" : UUID("b30978a7-cbbc-4c46-9eef-c90b21eecdfd") }
MongoDB server version: 4.2.18-rc0
Server has startup warnings:
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten]
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten] ** WARNING: Access control is not enabled for the database.
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten] **          Read and write access to data and configuration is
unrestricted.
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten]
---
Enable MongoDB's free cloud-based monitoring service, which will then receive and display
metrics about your deployment (disk utilization, CPU, operation statistics, etc).

The monitoring data will be available on a MongoDB website with a unique URL accessible to you
and anyone you share the URL with. MongoDB may use this information to make product
improvements and to suggest MongoDB products and deployment options to you.

To enable free monitoring, run the following command: db.enableFreeMonitoring()
To permanently disable this reminder, run the following command: db.disableFreeMonitoring()
---

> use test
switched to db test
> show collections;
movie
> db.find().pretty();
2022-11-24T23:26:58.414+0530 E  QUERY    [js] uncaught exception: TypeError: db.find is not a function :
@(shell):1:1
> db.movie.find().pretty();
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
{
        "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"),
        "name" : "newton",
        "ticket_no" : 690,
        "actor" : [
                "Rajkumar Rao",
                "Pankaj Tripathi"
        ],
        "price" : 310,
        "lastmodified" : ISODate("2019-09-28T14:47:49.204Z")
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
{
        "_id" : ObjectId("5d89e9adfd4adc2f84279f43"),
        "name" : "chichore",
        "price" : 274,
        "rating" : 4.3,
        "actor" : [
                "sushant",
                "shradha kapoor",
                "zzz",
                "harshal"
        ]
}
{
        "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"),
        "name" : "dream girl",
        "actor" : [
                "ayushman",
                "nushrat bharucha"
        ],
        "price" : 250,
        "rating" : null
}
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{
        "_id" : ObjectId("5ca456072952ebdd7ae2a930"),
        "name" : "paa",
        "actor" : [
                "Amitabh",
                "vidya balan",
                "Abhishek"
        ],
        "rating" : 2,
        "price" : 270,
        "ticket_no" : 210,
        "rdate" : ISODate("2019-01-23T00:00:00Z"),
        "others" : {
                "director" : "R Balki",
                "songs" : "Amit trivedi"
        }
}
> db.collections.count();
0
> db.collection.count();
0
> db;
test
> exit
bye
PS C:\Users\admin> mongo
MongoDB shell version v4.2.18-rc0
connecting to: mongodb://127.0.0.1:27017/?compressors=disabled&gssapiServiceName=mongodb
Implicit session: session { "id" : UUID("9ffb3b92-22d2-4637-9e36-65e01fca4bae") }
MongoDB server version: 4.2.18-rc0
Server has startup warnings:
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten]
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten] ** WARNING: Access control is not enabled for the database.
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten] **          Read and write access to data and configuration is
unrestricted.
2022-11-24T02:53:44.809+0530 I  CONTROL  [initandlisten]
---
Enable MongoDB's free cloud-based monitoring service, which will then receive and display
metrics about your deployment (disk utilization, CPU, operation statistics, etc).

The monitoring data will be available on a MongoDB website with a unique URL accessible to you
and anyone you share the URL with. MongoDB may use this information to make product
improvements and to suggest MongoDB products and deployment options to you.

To enable free monitoring, run the following command: db.enableFreeMonitoring()
To permanently disable this reminder, run the following command: db.disableFreeMonitoring()
---

> show dbs;
admin   0.000GB
blog    0.000GB
config  0.000GB
knowit  0.000GB
local   0.000GB
test    0.000GB
> use test;
switched to db test
> show collections;
movie
> show movie;
2022-11-24T23:32:37.698+0530 E  QUERY    [js] uncaught exception: Error: don't know how to show [movie] :
shellHelper.show@src/mongo/shell/utils.js:1139:11
shellHelper@src/mongo/shell/utils.js:790:15
@(shellhelp2):1:1
> show collections;
movie
> db.movie.find().pretty();
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
{
        "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"),
        "name" : "newton",
        "ticket_no" : 690,
        "actor" : [
                "Rajkumar Rao",
                "Pankaj Tripathi"
        ],
        "price" : 310,
        "lastmodified" : ISODate("2019-09-28T14:47:49.204Z")
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
{
        "_id" : ObjectId("5d89e9adfd4adc2f84279f43"),
        "name" : "chichore",
        "price" : 274,
        "rating" : 4.3,
        "actor" : [
                "sushant",
                "shradha kapoor",
                "zzz",
                "harshal"
        ]
}
{
        "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"),
        "name" : "dream girl",
        "actor" : [
                "ayushman",
                "nushrat bharucha"
        ],
        "price" : 250,
        "rating" : null
}
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{
        "_id" : ObjectId("5ca456072952ebdd7ae2a930"),
        "name" : "paa",
        "actor" : [
                "Amitabh",
                "vidya balan",
                "Abhishek"
        ],
        "rating" : 2,
        "price" : 270,
        "ticket_no" : 210,
        "rdate" : ISODate("2019-01-23T00:00:00Z"),
        "others" : {
                "director" : "R Balki",
                "songs" : "Amit trivedi"
        }
}
> db.inventory.find( {} );
> db.movie.find( {} );
{ "_id" : ObjectId("5aaa31a2639395f86922a87e"), "name" : "kahani", "actor" : [ "aaaa", "bbbb", "karan", "karri", "vidya"
 ], "ticket_no" : 420, "price" : 200, "ac7tors" : [ "bbbb" ], "rating" : 8, "lastmodified" : ISODate("2019-04-07T11:25:4
0.634Z") }
{ "_id" : ObjectId("5aaa3334639395f86922a880"), "name" : "lagaan", "actor" : [ "amir", "angraz" ], "rating" : 6, "ticket
_no" : 410, "price" : 350, "cancellation" : { "date" : Timestamp(1554356003, 1), "reason" : "user request" }, "lastModif
ied" : ISODate("2019-04-04T05:33:23.022Z") }
{ "_id" : ObjectId("5aaa31ee639395f86922a87f"), "name" : "3 idiots", "actor" : [ "Kareena Kapoor", "amir", "kareena", "m
ahadavan", "sharman" ], "rating" : 3, "ticket_no" : 150, "price" : 200 }
{ "_id" : ObjectId("5aaa3334639395f86922a882"), "name" : "aradhana", "actor" : [ "amitabh", "prem", "rajesh khanna" ], "
rating" : 3, "ticket_no" : 550, "price" : 260 }
{ "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"), "name" : "Andhadhund", "price" : 400, "actor" : [ "Ayushman", "radhika"
], "rating" : 4 }
{ "_id" : ObjectId("5aab6da4639395f86922a883"), "name" : "kahani 2", "ticket_no" : 820, "actor" : [ "vidya", "Arjun", "J
onny", "nawaz", "prasad", "Shreyas", "Jonny", "yash" ], "rating" : 5, "price" : 200 }
{ "_id" : ObjectId("5aaa3334639395f86922a881"), "name" : "sholay", "actor" : [ "Dharamendra", "Amitabh", "Sachin Pilgaok
ar", "Dharamendra", "Dharamendra", "Mr. Khote", "jaya bacchan", "sanjiv kapoor" ], "rating" : 6, "ticket_no" : 550, "pri
ce" : 350, "position" : [ 2, 2 ] }
{ "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"), "name" : "Andhadhund", "price" : null, "actor" : [ "Tabbu" ], "rating" :
 4 }
{ "_id" : ObjectId("5c8283789eb55675f0272933"), "name" : "uri", "rating" : 5, "actor" : [ "vicky kaushal", "yami", "Pare
sh Rawal" ] }
{ "_id" : ObjectId("5c865923d82c19b8ed996550"), "name" : "Dil dhadakane do", "rating" : 3, "price" : 340, "actor" : "['A
nil kapoor']" }
{ "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"), "name" : "newton", "ticket_no" : 690, "actor" : [ "Rajkumar Rao", "Panka
j Tripathi" ], "price" : 310, "lastmodified" : ISODate("2019-09-28T14:47:49.204Z") }
{ "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"), "name" : "Kesari", "actor" : [ "Akshay Kumar", "Pariniti chopra" ], "rat
ing" : 6, "price" : 350, "ticket_no" : 270, "rdate" : ISODate("2019-01-23T00:00:00Z") }
{ "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"), "name" : "padmavat", "rating" : 4, "price" : 250, "ticket_no" : 300, "ac
tor" : [ "Deepika", "shahid kapoor", "ranveer singh", "aditi Rao", "aaaaa" ], "cancellation" : { "date" : Timestamp(1567
175239, 1) } }
{ "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"), "name" : "mission mangal", "price" : 350, "actor" : [ "Sonakshi", "Vidya
 Balan" ], "rating" : 6 }
{ "_id" : ObjectId("5d89e9adfd4adc2f84279f43"), "name" : "chichore", "price" : 274, "rating" : 4.3, "actor" : [ "sushant
", "shradha kapoor", "zzz", "harshal" ] }
{ "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"), "name" : "dream girl", "actor" : [ "ayushman", "nushrat bharucha" ], "pr
ice" : 250, "rating" : null }
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{ "_id" : ObjectId("5ca456072952ebdd7ae2a930"), "name" : "paa", "actor" : [ "Amitabh", "vidya balan", "Abhishek" ], "rat
ing" : 2, "price" : 270, "ticket_no" : 210, "rdate" : ISODate("2019-01-23T00:00:00Z"), "others" : { "director" : "R Balk
i", "songs" : "Amit trivedi" } }
> db.movie.find( {} ).pretty();
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
{
        "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"),
        "name" : "newton",
        "ticket_no" : 690,
        "actor" : [
                "Rajkumar Rao",
                "Pankaj Tripathi"
        ],
        "price" : 310,
        "lastmodified" : ISODate("2019-09-28T14:47:49.204Z")
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
{
        "_id" : ObjectId("5d89e9adfd4adc2f84279f43"),
        "name" : "chichore",
        "price" : 274,
        "rating" : 4.3,
        "actor" : [
                "sushant",
                "shradha kapoor",
                "zzz",
                "harshal"
        ]
}
{
        "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"),
        "name" : "dream girl",
        "actor" : [
                "ayushman",
                "nushrat bharucha"
        ],
        "price" : 250,
        "rating" : null
}
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{
        "_id" : ObjectId("5ca456072952ebdd7ae2a930"),
        "name" : "paa",
        "actor" : [
                "Amitabh",
                "vidya balan",
                "Abhishek"
        ],
        "rating" : 2,
        "price" : 270,
        "ticket_no" : 210,
        "rdate" : ISODate("2019-01-23T00:00:00Z"),
        "others" : {
                "director" : "R Balki",
                "songs" : "Amit trivedi"
        }
}
> db.movie.find({name:'dream girl'});
{ "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"), "name" : "dream girl", "actor" : [ "ayushman", "nushrat bharucha" ], "pr
ice" : 250, "rating" : null }
> db.movie.find({name:'dream girl'})pretty();
2022-11-24T23:47:21.468+0530 E  QUERY    [js] uncaught exception: SyntaxError: unexpected token: identifier :
@(shell):1:34
> db.movie.find({name:'dream girl'}).pretty();
{
        "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"),
        "name" : "dream girl",
        "actor" : [
                "ayushman",
                "nushrat bharucha"
        ],
        "price" : 250,
        "rating" : null
}
> db.movie.find({actor:'nurshat'}).pretty();
>
> db.movie.find({actor:'nurshat'}).pretty();
> db.movie.find({name:'paa'},{_id:0,name:1,actor:1,rating:1});
{ "name" : "paa", "actor" : [ "Amitabh", "vidya balan", "Abhishek" ], "rating" : 2 }
> db.movie.find();
{ "_id" : ObjectId("5aaa31a2639395f86922a87e"), "name" : "kahani", "actor" : [ "aaaa", "bbbb", "karan", "karri", "vidya"
 ], "ticket_no" : 420, "price" : 200, "ac7tors" : [ "bbbb" ], "rating" : 8, "lastmodified" : ISODate("2019-04-07T11:25:4
0.634Z") }
{ "_id" : ObjectId("5aaa3334639395f86922a880"), "name" : "lagaan", "actor" : [ "amir", "angraz" ], "rating" : 6, "ticket
_no" : 410, "price" : 350, "cancellation" : { "date" : Timestamp(1554356003, 1), "reason" : "user request" }, "lastModif
ied" : ISODate("2019-04-04T05:33:23.022Z") }
{ "_id" : ObjectId("5aaa31ee639395f86922a87f"), "name" : "3 idiots", "actor" : [ "Kareena Kapoor", "amir", "kareena", "m
ahadavan", "sharman" ], "rating" : 3, "ticket_no" : 150, "price" : 200 }
{ "_id" : ObjectId("5aaa3334639395f86922a882"), "name" : "aradhana", "actor" : [ "amitabh", "prem", "rajesh khanna" ], "
rating" : 3, "ticket_no" : 550, "price" : 260 }
{ "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"), "name" : "Andhadhund", "price" : 400, "actor" : [ "Ayushman", "radhika"
], "rating" : 4 }
{ "_id" : ObjectId("5aab6da4639395f86922a883"), "name" : "kahani 2", "ticket_no" : 820, "actor" : [ "vidya", "Arjun", "J
onny", "nawaz", "prasad", "Shreyas", "Jonny", "yash" ], "rating" : 5, "price" : 200 }
{ "_id" : ObjectId("5aaa3334639395f86922a881"), "name" : "sholay", "actor" : [ "Dharamendra", "Amitabh", "Sachin Pilgaok
ar", "Dharamendra", "Dharamendra", "Mr. Khote", "jaya bacchan", "sanjiv kapoor" ], "rating" : 6, "ticket_no" : 550, "pri
ce" : 350, "position" : [ 2, 2 ] }
{ "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"), "name" : "Andhadhund", "price" : null, "actor" : [ "Tabbu" ], "rating" :
 4 }
{ "_id" : ObjectId("5c8283789eb55675f0272933"), "name" : "uri", "rating" : 5, "actor" : [ "vicky kaushal", "yami", "Pare
sh Rawal" ] }
{ "_id" : ObjectId("5c865923d82c19b8ed996550"), "name" : "Dil dhadakane do", "rating" : 3, "price" : 340, "actor" : "['A
nil kapoor']" }
{ "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"), "name" : "newton", "ticket_no" : 690, "actor" : [ "Rajkumar Rao", "Panka
j Tripathi" ], "price" : 310, "lastmodified" : ISODate("2019-09-28T14:47:49.204Z") }
{ "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"), "name" : "Kesari", "actor" : [ "Akshay Kumar", "Pariniti chopra" ], "rat
ing" : 6, "price" : 350, "ticket_no" : 270, "rdate" : ISODate("2019-01-23T00:00:00Z") }
{ "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"), "name" : "padmavat", "rating" : 4, "price" : 250, "ticket_no" : 300, "ac
tor" : [ "Deepika", "shahid kapoor", "ranveer singh", "aditi Rao", "aaaaa" ], "cancellation" : { "date" : Timestamp(1567
175239, 1) } }
{ "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"), "name" : "mission mangal", "price" : 350, "actor" : [ "Sonakshi", "Vidya
 Balan" ], "rating" : 6 }
{ "_id" : ObjectId("5d89e9adfd4adc2f84279f43"), "name" : "chichore", "price" : 274, "rating" : 4.3, "actor" : [ "sushant
", "shradha kapoor", "zzz", "harshal" ] }
{ "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"), "name" : "dream girl", "actor" : [ "ayushman", "nushrat bharucha" ], "pr
ice" : 250, "rating" : null }
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{ "_id" : ObjectId("5ca456072952ebdd7ae2a930"), "name" : "paa", "actor" : [ "Amitabh", "vidya balan", "Abhishek" ], "rat
ing" : 2, "price" : 270, "ticket_no" : 210, "rdate" : ISODate("2019-01-23T00:00:00Z"), "others" : { "director" : "R Balk
i", "songs" : "Amit trivedi" } }
> db.movie.find({name:'dream'},{_id:0,name:1,actor:1});
> db.inventory.find( { tags: { $all: ["red", "blank"] } } )
> db.inventory.find( { tags: { $all: ["red", "blank"] } } )
> db.inventory.find( { tags: { $all: ["red", "blank"] } } )
> db.inventory.find( { tags: { $all: ["red", "blank"] } } )
> db.movie.find().pretty();
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
{
        "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"),
        "name" : "newton",
        "ticket_no" : 690,
        "actor" : [
                "Rajkumar Rao",
                "Pankaj Tripathi"
        ],
        "price" : 310,
        "lastmodified" : ISODate("2019-09-28T14:47:49.204Z")
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
{
        "_id" : ObjectId("5d89e9adfd4adc2f84279f43"),
        "name" : "chichore",
        "price" : 274,
        "rating" : 4.3,
        "actor" : [
                "sushant",
                "shradha kapoor",
                "zzz",
                "harshal"
        ]
}
{
        "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"),
        "name" : "dream girl",
        "actor" : [
                "ayushman",
                "nushrat bharucha"
        ],
        "price" : 250,
        "rating" : null
}
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{
        "_id" : ObjectId("5ca456072952ebdd7ae2a930"),
        "name" : "paa",
        "actor" : [
                "Amitabh",
                "vidya balan",
                "Abhishek"
        ],
        "rating" : 2,
        "price" : 270,
        "ticket_no" : 210,
        "rdate" : ISODate("2019-01-23T00:00:00Z"),
        "others" : {
                "director" : "R Balki",
                "songs" : "Amit trivedi"
        }
}
> db.find({rating:6});
2022-11-24T23:56:30.434+0530 E  QUERY    [js] uncaught exception: TypeError: db.find is not a function :
@(shell):1:1
> db.find({rating:'6'});
2022-11-24T23:57:15.090+0530 E  QUERY    [js] uncaught exception: TypeError: db.find is not a function :
@(shell):1:1
> db.movie.find({rating:'6'});
> db.movie.find({rating:'2'});
> db.movie.find({"rating":2});
{ "_id" : ObjectId("5ca456072952ebdd7ae2a930"), "name" : "paa", "actor" : [ "Amitabh", "vidya balan", "Abhishek" ], "rat
ing" : 2, "price" : 270, "ticket_no" : 210, "rdate" : ISODate("2019-01-23T00:00:00Z"), "others" : { "director" : "R Balk
i", "songs" : "Amit trivedi" } }
> db.movie.find({"rating":3});
{ "_id" : ObjectId("5aaa31ee639395f86922a87f"), "name" : "3 idiots", "actor" : [ "Kareena Kapoor", "amir", "kareena", "m
ahadavan", "sharman" ], "rating" : 3, "ticket_no" : 150, "price" : 200 }
{ "_id" : ObjectId("5aaa3334639395f86922a882"), "name" : "aradhana", "actor" : [ "amitabh", "prem", "rajesh khanna" ], "
rating" : 3, "ticket_no" : 550, "price" : 260 }
{ "_id" : ObjectId("5c865923d82c19b8ed996550"), "name" : "Dil dhadakane do", "rating" : 3, "price" : 340, "actor" : "['A
nil kapoor']" }
> db.movie.find({"rating":3}).pretty();
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
> db.movie.find({rating:3}).pretty();
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
> db.movie.find({rating:2, price:250},{_id:0,name:1});
> db.movie.find({rating:3, price:250},{_id:0,name:1});
> db.movie.find({rating:3, price:350},{_id:0,name:1});
> db.movie.find({rating:3, price:200},{_id:0,name:1});
{ "name" : "3 idiots" }
> db.movie.find({rating:{$gt:3}, price:200},{_id:0,name:1});
{ "name" : "kahani" }
{ "name" : "kahani 2" }
> db.movie.find({price:{$in:[250, 300,350]}, {name:1, _id:0});
...
...
>  db.movie.find({price:{$in:[250, 300,350]}, {name:1, _id:0}});
2022-11-25T01:21:42.965+0530 E  QUERY    [js] uncaught exception: SyntaxError: expected property name, got '{' :
@(shell):1:43
> db.movie.find({price:{$in:[250, 300,350]}}, {name:1, _id:0});
{ "name" : "lagaan" }
{ "name" : "sholay" }
{ "name" : "Kesari" }
{ "name" : "padmavat" }
{ "name" : "mission mangal" }
{ "name" : "dream girl" }
> db.movie.find($or:[{rating:4}, {price:{$gt:350}}]);
2022-11-25T01:28:30.858+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:17
> db.movie.find({$or:[{rating:4}, {price:{$gt:350}}]});
{ "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"), "name" : "Andhadhund", "price" : 400, "actor" : [ "Ayushman", "radhika"
], "rating" : 4 }
{ "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"), "name" : "Andhadhund", "price" : null, "actor" : [ "Tabbu" ], "rating" :
 4 }
{ "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"), "name" : "padmavat", "rating" : 4, "price" : 250, "ticket_no" : 300, "ac
tor" : [ "Deepika", "shahid kapoor", "ranveer singh", "aditi Rao", "aaaaa" ], "cancellation" : { "date" : Timestamp(1567
175239, 1) } }
> db.movie.find({$or:[{rating:4}, {price:350}]});
{ "_id" : ObjectId("5aaa3334639395f86922a880"), "name" : "lagaan", "actor" : [ "amir", "angraz" ], "rating" : 6, "ticket
_no" : 410, "price" : 350, "cancellation" : { "date" : Timestamp(1554356003, 1), "reason" : "user request" }, "lastModif
ied" : ISODate("2019-04-04T05:33:23.022Z") }
{ "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"), "name" : "Andhadhund", "price" : 400, "actor" : [ "Ayushman", "radhika"
], "rating" : 4 }
{ "_id" : ObjectId("5aaa3334639395f86922a881"), "name" : "sholay", "actor" : [ "Dharamendra", "Amitabh", "Sachin Pilgaok
ar", "Dharamendra", "Dharamendra", "Mr. Khote", "jaya bacchan", "sanjiv kapoor" ], "rating" : 6, "ticket_no" : 550, "pri
ce" : 350, "position" : [ 2, 2 ] }
{ "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"), "name" : "Andhadhund", "price" : null, "actor" : [ "Tabbu" ], "rating" :
 4 }
{ "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"), "name" : "Kesari", "actor" : [ "Akshay Kumar", "Pariniti chopra" ], "rat
ing" : 6, "price" : 350, "ticket_no" : 270, "rdate" : ISODate("2019-01-23T00:00:00Z") }
{ "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"), "name" : "padmavat", "rating" : 4, "price" : 250, "ticket_no" : 300, "ac
tor" : [ "Deepika", "shahid kapoor", "ranveer singh", "aditi Rao", "aaaaa" ], "cancellation" : { "date" : Timestamp(1567
175239, 1) } }
{ "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"), "name" : "mission mangal", "price" : 350, "actor" : [ "Sonakshi", "Vidya
 Balan" ], "rating" : 6 }
> db.movie.find({$or:[{rating:4}, {price:350}]}).pretty();
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
> db.movie.find({$or:[{rating:4}, {price:{$gt:350}}]}).pretty();
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
> db.movie.find({$not:{price:{$gt:200, $lt:400}}}).pretty();
Error: error: {
        "ok" : 0,
        "errmsg" : "unknown top level operator: $not",
        "code" : 2,
        "codeName" : "BadValue"
}
> db.movie.find({price:{$not{{gt:200, $lt:400}}}}).pretty();
2022-11-25T01:33:45.470+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing : after property id :
@(shell):1:26
> db.movie.find(price:{$not{{gt:200, $lt:400}}}).pretty();
2022-11-25T01:33:51.710+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:19
> db.movie.find(price:{$not{gt:200, $lt:400}}).pretty();
2022-11-25T01:34:13.310+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:19
> db.movie.find({price:{$not{gt:200, $lt:400}}}).pretty();
2022-11-25T01:34:34.222+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing : after property id :
@(shell):1:26
> db.movie.find(price:{$not{gt:200, $lt:400}}).pretty();
2022-11-25T01:34:42.910+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:19
> db.movie.find(price:$not{gt:200, $lt:400}).pretty();
2022-11-25T01:35:05.279+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:19
> db.movie.find(price:$not[{gt:200, $lt:400}]).pretty();
2022-11-25T01:35:56.991+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:19
> db.movie.find(price:{$not[{gt:200, $lt:400}]}).pretty();
2022-11-25T01:36:23.775+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:19
> db.movie.find({$not: [price:{gt:200, $lt:400}]}).pretty();
2022-11-25T01:37:55.056+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ] after element list :
@(shell):1:27
> db.movie.find(price:{$not:{gt:200, $lt:400}}).pretty();
2022-11-25T01:38:49.825+0530 E  QUERY    [js] uncaught exception: SyntaxError: missing ) after argument list :
@(shell):1:19
> db.movie.find({price:{$not:{gt:200, $lt:400}}}).pretty();
Error: error: {
        "ok" : 0,
        "errmsg" : "unknown operator: gt",
        "code" : 2,
        "codeName" : "BadValue"
}
> db.movie.find({price:{$not:{$gt:200, $lt:400}}}).pretty();
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
> db.movie.find({price:{$not:{$gt:200, $lt:400}}}).pretty();
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
> db.movie.find({rating:{$mod:[2,0]}).pretty();
...
...
> db.movie.find({rating:{$mod:[2,0]}}).pretty();
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
{
        "_id" : ObjectId("5d89e9adfd4adc2f84279f43"),
        "name" : "chichore",
        "price" : 274,
        "rating" : 4.3,
        "actor" : [
                "sushant",
                "shradha kapoor",
                "zzz",
                "harshal"
        ]
}
{
        "_id" : ObjectId("5ca456072952ebdd7ae2a930"),
        "name" : "paa",
        "actor" : [
                "Amitabh",
                "vidya balan",
                "Abhishek"
        ],
        "rating" : 2,
        "price" : 270,
        "ticket_no" : 210,
        "rdate" : ISODate("2019-01-23T00:00:00Z"),
        "others" : {
                "director" : "R Balki",
                "songs" : "Amit trivedi"
        }
}
> db.movie.find({actor:'Amitabh'}, {name:1, _id:0});
{ "name" : "sholay" }
{ "name" : "paa" }
> db.movie.find().sort({name})'
2022-11-25T01:43:16.020+0530 E  QUERY    [js] uncaught exception: SyntaxError: '' literal not terminated before end of s
cript :
@(shell):1:29
> db.movie.find().sort({name});
2022-11-25T01:43:17.636+0530 E  QUERY    [js] uncaught exception: ReferenceError: name is not defined :
@(shell):1:23
> db.movie.find().sort("name");
Error: error: {
        "ok" : 0,
        "errmsg" : "Failed to parse: sort: \"name\". 'sort' field must be of BSON type object.",
        "code" : 9,
        "codeName" : "FailedToParse"
}
> db.movie.find().sort({name:1});
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{ "_id" : ObjectId("5aaa31ee639395f86922a87f"), "name" : "3 idiots", "actor" : [ "Kareena Kapoor", "amir", "kareena", "m
ahadavan", "sharman" ], "rating" : 3, "ticket_no" : 150, "price" : 200 }
{ "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"), "name" : "Andhadhund", "price" : 400, "actor" : [ "Ayushman", "radhika"
], "rating" : 4 }
{ "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"), "name" : "Andhadhund", "price" : null, "actor" : [ "Tabbu" ], "rating" :
 4 }
{ "_id" : ObjectId("5c865923d82c19b8ed996550"), "name" : "Dil dhadakane do", "rating" : 3, "price" : 340, "actor" : "['A
nil kapoor']" }
{ "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"), "name" : "Kesari", "actor" : [ "Akshay Kumar", "Pariniti chopra" ], "rat
ing" : 6, "price" : 350, "ticket_no" : 270, "rdate" : ISODate("2019-01-23T00:00:00Z") }
{ "_id" : ObjectId("5aaa3334639395f86922a882"), "name" : "aradhana", "actor" : [ "amitabh", "prem", "rajesh khanna" ], "
rating" : 3, "ticket_no" : 550, "price" : 260 }
{ "_id" : ObjectId("5d89e9adfd4adc2f84279f43"), "name" : "chichore", "price" : 274, "rating" : 4.3, "actor" : [ "sushant
", "shradha kapoor", "zzz", "harshal" ] }
{ "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"), "name" : "dream girl", "actor" : [ "ayushman", "nushrat bharucha" ], "pr
ice" : 250, "rating" : null }
{ "_id" : ObjectId("5aaa31a2639395f86922a87e"), "name" : "kahani", "actor" : [ "aaaa", "bbbb", "karan", "karri", "vidya"
 ], "ticket_no" : 420, "price" : 200, "ac7tors" : [ "bbbb" ], "rating" : 8, "lastmodified" : ISODate("2019-04-07T11:25:4
0.634Z") }
{ "_id" : ObjectId("5aab6da4639395f86922a883"), "name" : "kahani 2", "ticket_no" : 820, "actor" : [ "vidya", "Arjun", "J
onny", "nawaz", "prasad", "Shreyas", "Jonny", "yash" ], "rating" : 5, "price" : 200 }
{ "_id" : ObjectId("5aaa3334639395f86922a880"), "name" : "lagaan", "actor" : [ "amir", "angraz" ], "rating" : 6, "ticket
_no" : 410, "price" : 350, "cancellation" : { "date" : Timestamp(1554356003, 1), "reason" : "user request" }, "lastModif
ied" : ISODate("2019-04-04T05:33:23.022Z") }
{ "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"), "name" : "mission mangal", "price" : 350, "actor" : [ "Sonakshi", "Vidya
 Balan" ], "rating" : 6 }
{ "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"), "name" : "newton", "ticket_no" : 690, "actor" : [ "Rajkumar Rao", "Panka
j Tripathi" ], "price" : 310, "lastmodified" : ISODate("2019-09-28T14:47:49.204Z") }
{ "_id" : ObjectId("5ca456072952ebdd7ae2a930"), "name" : "paa", "actor" : [ "Amitabh", "vidya balan", "Abhishek" ], "rat
ing" : 2, "price" : 270, "ticket_no" : 210, "rdate" : ISODate("2019-01-23T00:00:00Z"), "others" : { "director" : "R Balk
i", "songs" : "Amit trivedi" } }
{ "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"), "name" : "padmavat", "rating" : 4, "price" : 250, "ticket_no" : 300, "ac
tor" : [ "Deepika", "shahid kapoor", "ranveer singh", "aditi Rao", "aaaaa" ], "cancellation" : { "date" : Timestamp(1567
175239, 1) } }
{ "_id" : ObjectId("5aaa3334639395f86922a881"), "name" : "sholay", "actor" : [ "Dharamendra", "Amitabh", "Sachin Pilgaok
ar", "Dharamendra", "Dharamendra", "Mr. Khote", "jaya bacchan", "sanjiv kapoor" ], "rating" : 6, "ticket_no" : 550, "pri
ce" : 350, "position" : [ 2, 2 ] }
{ "_id" : ObjectId("5c8283789eb55675f0272933"), "name" : "uri", "rating" : 5, "actor" : [ "vicky kaushal", "yami", "Pare
sh Rawal" ] }
> db.movie.find().sort({name:1}).pretty();
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5d89e9adfd4adc2f84279f43"),
        "name" : "chichore",
        "price" : 274,
        "rating" : 4.3,
        "actor" : [
                "sushant",
                "shradha kapoor",
                "zzz",
                "harshal"
        ]
}
{
        "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"),
        "name" : "dream girl",
        "actor" : [
                "ayushman",
                "nushrat bharucha"
        ],
        "price" : 250,
        "rating" : null
}
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
{
        "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"),
        "name" : "newton",
        "ticket_no" : 690,
        "actor" : [
                "Rajkumar Rao",
                "Pankaj Tripathi"
        ],
        "price" : 310,
        "lastmodified" : ISODate("2019-09-28T14:47:49.204Z")
}
{
        "_id" : ObjectId("5ca456072952ebdd7ae2a930"),
        "name" : "paa",
        "actor" : [
                "Amitabh",
                "vidya balan",
                "Abhishek"
        ],
        "rating" : 2,
        "price" : 270,
        "ticket_no" : 210,
        "rdate" : ISODate("2019-01-23T00:00:00Z"),
        "others" : {
                "director" : "R Balki",
                "songs" : "Amit trivedi"
        }
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
> db.movie.find().sort({name:-1}).pretty();
{
        "_id" : ObjectId("5c8283789eb55675f0272933"),
        "name" : "uri",
        "rating" : 5,
        "actor" : [
                "vicky kaushal",
                "yami",
                "Paresh Rawal"
        ]
}
{
        "_id" : ObjectId("5aaa3334639395f86922a881"),
        "name" : "sholay",
        "actor" : [
                "Dharamendra",
                "Amitabh",
                "Sachin Pilgaokar",
                "Dharamendra",
                "Dharamendra",
                "Mr. Khote",
                "jaya bacchan",
                "sanjiv kapoor"
        ],
        "rating" : 6,
        "ticket_no" : 550,
        "price" : 350,
        "position" : [
                2,
                2
        ]
}
{
        "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"),
        "name" : "padmavat",
        "rating" : 4,
        "price" : 250,
        "ticket_no" : 300,
        "actor" : [
                "Deepika",
                "shahid kapoor",
                "ranveer singh",
                "aditi Rao",
                "aaaaa"
        ],
        "cancellation" : {
                "date" : Timestamp(1567175239, 1)
        }
}
{
        "_id" : ObjectId("5ca456072952ebdd7ae2a930"),
        "name" : "paa",
        "actor" : [
                "Amitabh",
                "vidya balan",
                "Abhishek"
        ],
        "rating" : 2,
        "price" : 270,
        "ticket_no" : 210,
        "rdate" : ISODate("2019-01-23T00:00:00Z"),
        "others" : {
                "director" : "R Balki",
                "songs" : "Amit trivedi"
        }
}
{
        "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"),
        "name" : "newton",
        "ticket_no" : 690,
        "actor" : [
                "Rajkumar Rao",
                "Pankaj Tripathi"
        ],
        "price" : 310,
        "lastmodified" : ISODate("2019-09-28T14:47:49.204Z")
}
{
        "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"),
        "name" : "mission mangal",
        "price" : 350,
        "actor" : [
                "Sonakshi",
                "Vidya Balan"
        ],
        "rating" : 6
}
{
        "_id" : ObjectId("5aaa3334639395f86922a880"),
        "name" : "lagaan",
        "actor" : [
                "amir",
                "angraz"
        ],
        "rating" : 6,
        "ticket_no" : 410,
        "price" : 350,
        "cancellation" : {
                "date" : Timestamp(1554356003, 1),
                "reason" : "user request"
        },
        "lastModified" : ISODate("2019-04-04T05:33:23.022Z")
}
{
        "_id" : ObjectId("5aab6da4639395f86922a883"),
        "name" : "kahani 2",
        "ticket_no" : 820,
        "actor" : [
                "vidya",
                "Arjun",
                "Jonny",
                "nawaz",
                "prasad",
                "Shreyas",
                "Jonny",
                "yash"
        ],
        "rating" : 5,
        "price" : 200
}
{
        "_id" : ObjectId("5aaa31a2639395f86922a87e"),
        "name" : "kahani",
        "actor" : [
                "aaaa",
                "bbbb",
                "karan",
                "karri",
                "vidya"
        ],
        "ticket_no" : 420,
        "price" : 200,
        "ac7tors" : [
                "bbbb"
        ],
        "rating" : 8,
        "lastmodified" : ISODate("2019-04-07T11:25:40.634Z")
}
{
        "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"),
        "name" : "dream girl",
        "actor" : [
                "ayushman",
                "nushrat bharucha"
        ],
        "price" : 250,
        "rating" : null
}
{
        "_id" : ObjectId("5d89e9adfd4adc2f84279f43"),
        "name" : "chichore",
        "price" : 274,
        "rating" : 4.3,
        "actor" : [
                "sushant",
                "shradha kapoor",
                "zzz",
                "harshal"
        ]
}
{
        "_id" : ObjectId("5aaa3334639395f86922a882"),
        "name" : "aradhana",
        "actor" : [
                "amitabh",
                "prem",
                "rajesh khanna"
        ],
        "rating" : 3,
        "ticket_no" : 550,
        "price" : 260
}
{
        "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"),
        "name" : "Kesari",
        "actor" : [
                "Akshay Kumar",
                "Pariniti chopra"
        ],
        "rating" : 6,
        "price" : 350,
        "ticket_no" : 270,
        "rdate" : ISODate("2019-01-23T00:00:00Z")
}
{
        "_id" : ObjectId("5c865923d82c19b8ed996550"),
        "name" : "Dil dhadakane do",
        "rating" : 3,
        "price" : 340,
        "actor" : "['Anil kapoor']"
}
{
        "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"),
        "name" : "Andhadhund",
        "price" : 400,
        "actor" : [
                "Ayushman",
                "radhika"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"),
        "name" : "Andhadhund",
        "price" : null,
        "actor" : [
                "Tabbu"
        ],
        "rating" : 4
}
{
        "_id" : ObjectId("5aaa31ee639395f86922a87f"),
        "name" : "3 idiots",
        "actor" : [
                "Kareena Kapoor",
                "amir",
                "kareena",
                "mahadavan",
                "sharman"
        ],
        "rating" : 3,
        "ticket_no" : 150,
        "price" : 200
}
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd"), "price" : 280 }
> db.movie.find({},{name:1}).sort({name:1}).pretty();
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd") }
{ "_id" : ObjectId("5aaa31ee639395f86922a87f"), "name" : "3 idiots" }
{ "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"), "name" : "Andhadhund" }
{ "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"), "name" : "Andhadhund" }
{ "_id" : ObjectId("5c865923d82c19b8ed996550"), "name" : "Dil dhadakane do" }
{ "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"), "name" : "Kesari" }
{ "_id" : ObjectId("5aaa3334639395f86922a882"), "name" : "aradhana" }
{ "_id" : ObjectId("5d89e9adfd4adc2f84279f43"), "name" : "chichore" }
{ "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"), "name" : "dream girl" }
{ "_id" : ObjectId("5aaa31a2639395f86922a87e"), "name" : "kahani" }
{ "_id" : ObjectId("5aab6da4639395f86922a883"), "name" : "kahani 2" }
{ "_id" : ObjectId("5aaa3334639395f86922a880"), "name" : "lagaan" }
{ "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"), "name" : "mission mangal" }
{ "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"), "name" : "newton" }
{ "_id" : ObjectId("5ca456072952ebdd7ae2a930"), "name" : "paa" }
{ "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"), "name" : "padmavat" }
{ "_id" : ObjectId("5aaa3334639395f86922a881"), "name" : "sholay" }
{ "_id" : ObjectId("5c8283789eb55675f0272933"), "name" : "uri" }
> db.movie.find({},{name:1}).sort({name:-1}).pretty();
{ "_id" : ObjectId("5c8283789eb55675f0272933"), "name" : "uri" }
{ "_id" : ObjectId("5aaa3334639395f86922a881"), "name" : "sholay" }
{ "_id" : ObjectId("5ca47e5b2952ebdd7ae2a931"), "name" : "padmavat" }
{ "_id" : ObjectId("5ca456072952ebdd7ae2a930"), "name" : "paa" }
{ "_id" : ObjectId("5ca47ef82952ebdd7ae2a932"), "name" : "newton" }
{ "_id" : ObjectId("5d6935a3470e2bef2a82cdfa"), "name" : "mission mangal" }
{ "_id" : ObjectId("5aaa3334639395f86922a880"), "name" : "lagaan" }
{ "_id" : ObjectId("5aab6da4639395f86922a883"), "name" : "kahani 2" }
{ "_id" : ObjectId("5aaa31a2639395f86922a87e"), "name" : "kahani" }
{ "_id" : ObjectId("5d8f51ce065d3e2aa902aa22"), "name" : "dream girl" }
{ "_id" : ObjectId("5d89e9adfd4adc2f84279f43"), "name" : "chichore" }
{ "_id" : ObjectId("5aaa3334639395f86922a882"), "name" : "aradhana" }
{ "_id" : ObjectId("5ca453ef2952ebdd7ae2a92f"), "name" : "Kesari" }
{ "_id" : ObjectId("5c865923d82c19b8ed996550"), "name" : "Dil dhadakane do" }
{ "_id" : ObjectId("5bf6a36f57b2d4cc676c7a95"), "name" : "Andhadhund" }
{ "_id" : ObjectId("5bf6a38c57b2d4cc676c7a96"), "name" : "Andhadhund" }
{ "_id" : ObjectId("5aaa31ee639395f86922a87f"), "name" : "3 idiots" }
{ "_id" : ObjectId("5d8f6eec620d2353221b91dd") }
> db.movie.find({},{name:1, _id:0}).sort({name:1}).pretty();
{ }
{ "name" : "3 idiots" }
{ "name" : "Andhadhund" }
{ "name" : "Andhadhund" }
{ "name" : "Dil dhadakane do" }
{ "name" : "Kesari" }
{ "name" : "aradhana" }
{ "name" : "chichore" }
{ "name" : "dream girl" }
{ "name" : "kahani" }
{ "name" : "kahani 2" }
{ "name" : "lagaan" }
{ "name" : "mission mangal" }
{ "name" : "newton" }
{ "name" : "paa" }
{ "name" : "padmavat" }
{ "name" : "sholay" }
{ "name" : "uri" }
> db.movie.find({},{name:1, _id:0}).sort({name:-1}).pretty();
{ "name" : "uri" }
{ "name" : "sholay" }
{ "name" : "padmavat" }
{ "name" : "paa" }
{ "name" : "newton" }
{ "name" : "mission mangal" }
{ "name" : "lagaan" }
{ "name" : "kahani 2" }
{ "name" : "kahani" }
{ "name" : "dream girl" }
{ "name" : "chichore" }
{ "name" : "aradhana" }
{ "name" : "Kesari" }
{ "name" : "Dil dhadakane do" }
{ "name" : "Andhadhund" }
{ "name" : "Andhadhund" }
{ "name" : "3 idiots" }
{ }
> db.movie.find({},
... db.movie.find({},{name:1, _id:0}).sort({name:1}).count();
...
...
> db.movie.find({},{name:1, _id:0}).count();
18
> db.movie.find({},
... {name:1, _id:0}).
... sort({name:1}).
... pretty();
{ }
{ "name" : "3 idiots" }
{ "name" : "Andhadhund" }
{ "name" : "Andhadhund" }
{ "name" : "Dil dhadakane do" }
{ "name" : "Kesari" }
{ "name" : "aradhana" }
{ "name" : "chichore" }
{ "name" : "dream girl" }
{ "name" : "kahani" }
{ "name" : "kahani 2" }
{ "name" : "lagaan" }
{ "name" : "mission mangal" }
{ "name" : "newton" }
{ "name" : "paa" }
{ "name" : "padmavat" }
{ "name" : "sholay" }
{ "name" : "uri" }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(1).skip(2).pretty();
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(2).skip(2).pretty();
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
{ "name" : "Andhadhund", "price" : null, "rating" : 4 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(3).skip(2).pretty();
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
{ "name" : "Andhadhund", "price" : null, "rating" : 4 }
{ "name" : "Dil dhadakane do", "rating" : 3, "price" : 340 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(3).skip(1).pretty();
{ "name" : "3 idiots", "rating" : 3, "price" : 200 }
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
{ "name" : "Andhadhund", "price" : null, "rating" : 4 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(3).skip(0).pretty();
{ "price" : 280 }
{ "name" : "3 idiots", "rating" : 3, "price" : 200 }
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(3).skip(2).pretty();
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
{ "name" : "Andhadhund", "price" : null, "rating" : 4 }
{ "name" : "Dil dhadakane do", "rating" : 3, "price" : 340 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(4).skip(2).pretty();
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
{ "name" : "Andhadhund", "price" : null, "rating" : 4 }
{ "name" : "Dil dhadakane do", "rating" : 3, "price" : 340 }
{ "name" : "Kesari", "rating" : 6, "price" : 350 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(4).pretty();
{ "price" : 280 }
{ "name" : "3 idiots", "rating" : 3, "price" : 200 }
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
{ "name" : "Andhadhund", "price" : null, "rating" : 4 }


> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).limit(1).skip(1).pretty();
{ "name" : "3 idiots", "rating" : 3, "price" : 200 }
> db.movie.find({}, {name:1, rating:1, price:1, _id:0}).sort({name:1}).pretty();
{ "price" : 280 }
{ "name" : "3 idiots", "rating" : 3, "price" : 200 }
{ "name" : "Andhadhund", "price" : 400, "rating" : 4 }
{ "name" : "Andhadhund", "price" : null, "rating" : 4 }
{ "name" : "Dil dhadakane do", "rating" : 3, "price" : 340 }
{ "name" : "Kesari", "rating" : 6, "price" : 350 }
{ "name" : "aradhana", "rating" : 3, "price" : 260 }
{ "name" : "chichore", "price" : 274, "rating" : 4.3 }
{ "name" : "dream girl", "price" : 250, "rating" : null }
{ "name" : "kahani", "price" : 200, "rating" : 8 }
{ "name" : "kahani 2", "rating" : 5, "price" : 200 }
{ "name" : "lagaan", "rating" : 6, "price" : 350 }
{ "name" : "mission mangal", "price" : 350, "rating" : 6 }
{ "name" : "newton", "price" : 310 }
{ "name" : "paa", "rating" : 2, "price" : 270 }
{ "name" : "padmavat", "rating" : 4, "price" : 250 }
{ "name" : "sholay", "rating" : 6, "price" : 350 }
{ "name" : "uri", "rating" : 5 }
>