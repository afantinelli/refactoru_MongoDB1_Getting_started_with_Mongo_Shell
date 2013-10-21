completed all of the 11 steps in Part 1 of the MongoDB1 exercise - no code to commit since exercise was done in terminal.
below is what I did in terminal:

Admins-Mac-mini-3:~ RU-011$ sudo mongo
Password:
MongoDB shell version: 2.4.6
connecting to: test
Server has startup warnings: 
Mon Oct 21 11:28:10.526 [initandlisten] 
Mon Oct 21 11:28:10.526 [initandlisten] ** WARNING: soft rlimits too low. Number of files is 256, should be at least 1000
> db.createCollection('students')
{ "ok" : 1 }
> show collections
students
system.indexes
> db.students.insert({name : "Allan"}, {name : "Megan"}, {name : "Lily"})
> show collections
students
system.indexes
> db.students.insert({name : "Allan"}
... db.students.insert({name : "Allan"})
... 

> db.students.insert({name : "Allan"})
> db.students.insert({name : "Megan"})
> db.students.insert({name : "Lily"})
> db.students.findOne({name : "Allan"})
{ "_id" : ObjectId("52656b85a2fafe2211dd8bb2"), "name" : "Allan" }
> db.students.save({name : "Ya Mar"})
> db.students.find()
{ "_id" : ObjectId("52656b85a2fafe2211dd8bb2"), "name" : "Allan" }
{ "_id" : ObjectId("52656bc7a2fafe2211dd8bb3"), "name" : "Allan" }
{ "_id" : ObjectId("52656bd4a2fafe2211dd8bb4"), "name" : "Megan" }
{ "_id" : ObjectId("52656bdca2fafe2211dd8bb5"), "name" : "Lily" }
{ "_id" : ObjectId("52656c13a2fafe2211dd8bb6"), "name" : "Ya Mar" }
> db.students.remove({name : "Allan"})
> db.students.find()
{ "_id" : ObjectId("52656bd4a2fafe2211dd8bb4"), "name" : "Megan" }
{ "_id" : ObjectId("52656bdca2fafe2211dd8bb5"), "name" : "Lily" }
{ "_id" : ObjectId("52656c13a2fafe2211dd8bb6"), "name" : "Ya Mar" }
> db.students.remove()
> db.students.find()
> 
bye
