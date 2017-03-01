# mongodb-query
1.use academic  
2.show collections
3.use academic
4.db.createCollection('department')
5.db.createCollection('student')
6.db.getCollectionInfos({name: 'student'})
7.db.department.insertMany([
    {code:'DP01', name:'Departemen Pertanian', major:'Kelas Teri'},
    {code:'DP02', name:'Departemen Ekonomi', major:'Kelas Kakap'},
    {code:'DP03', name:'Departemen Sains Komputer', major:'Kelas Tinju'},
    {code:'DP04', name:'Departemen Kedokteran', major:'Kelas Berat'},
    {code:'DP05', name:'Departemen Hukum', major:'Kelas Ogahogahan'}
],{ordered: true})  
8.db.student.insertMany([
    {studentId:'ST01', name:'Danang Aji Tamtomo', address:'Duta Bintaro', department:{ "$ref" : "department", "$id" : ObjectId("58b65103da5e94cffe5f1f19"), "$db" : "academic" }},
    {studentId:'ST02', name:'Firman', address:'Belakang delta', department:{ "$ref" : "department", "$id" : ObjectId("58b65103da5e94cffe5f1f18"), "$db" : "academic" }},
    {studentId:'ST03', name:'Adam', address:'Dalem delta', department:{ "$ref" : "department", "$id" : ObjectId("58b65103da5e94cffe5f1f1a"), "$db" : "academic" }},
],{ordered: true})
9.db.getCollection('student').find({})
10.db.student.find({})
11.
12.
13.
14.
