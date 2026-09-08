# MongoDB
Atlas atlas-3m3ssv-shard-0 [primary] test> db.students.insertMany([
|     {
|         rollNo: 101,
|         name: "Vasanth",
|         age: 21,
|         department: "CSE",
|         marks: 85,
|         skills: ["Java", "Python", "MongoDB"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 102,
|         name: "Rahul",
|         age: 22,
|         department: "ECE",
|         marks: 72,
|         skills: ["C", "Python", "Arduino"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 103,
|         name: "Priya",
|         age: 20,
|         department: "CSE",
|         marks: 91,
|         skills: ["Java", "Python", "AI"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 104,
|         name: "Arjun",
|         age: 23,
|         department: "MECH",
|         marks: 68,
|         skills: ["AutoCAD", "C", "Java"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         }
|     },
|
|     {
|         rollNo: 105,
|         name: "Sneha",
|         age: 21,
|         department: "IT",
|         marks: 88,
|         skills: ["Python", "MongoDB", "HTML"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 106,
|         name: "Kiran",
|         age: 24,
|         department: "EEE",
|         marks: 65,
|         skills: ["C", "Arduino", "MATLAB"],
|         address: {
|             city: "Pune",
|             state: "Maharashtra"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 107,
|         name: "Anjali",
|         age: 20,
|         department: "CSE",
|         marks: 95,
|         skills: ["Java", "Python", "AI", "MongoDB"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 108,
|         name: "Rohit",
|         age: 22,
|         department: "IT",
|         marks: 76,
|         skills: ["JavaScript", "HTML", "CSS"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 109,
|         name: "Divya",
|         age: 21,
|         department: "CSE",
|         marks: 89,
|         skills: ["Python", "MongoDB", "Java"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 110,
|         name: "Suresh",
|         age: 23,
|         department: "CIVIL",
|         marks: 70,
|         skills: ["AutoCAD", "C", "STAAD"],
|         address: {
|             city: "Vijayawada",
|             state: "Andhra Pradesh"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 111,
|         name: "Meena",
|         age: 22,
|         department: "ECE",
|         marks: 82,
|         skills: ["Python", "Arduino", "IoT"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 112,
|         name: "Akash",
|         age: 25,
|         department: "CSE",
|         marks: 60,
|         skills: ["C", "Java"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         },
|         scholarship: false
|     }
| ])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6a9fb0fc4cfe5f91e2977bcc'),
    '1': ObjectId('6a9fb0fc4cfe5f91e2977bcd'),
    '2': ObjectId('6a9fb0fc4cfe5f91e2977bce'),
    '3': ObjectId('6a9fb0fc4cfe5f91e2977bcf'),
    '4': ObjectId('6a9fb0fc4cfe5f91e2977bd0'),
    '5': ObjectId('6a9fb0fc4cfe5f91e2977bd1'),
    '6': ObjectId('6a9fb0fc4cfe5f91e2977bd2'),
    '7': ObjectId('6a9fb0fc4cfe5f91e2977bd3'),
    '8': ObjectId('6a9fb0fc4cfe5f91e2977bd4'),
    '9': ObjectId('6a9fb0fc4cfe5f91e2977bd5'),
    '10': ObjectId('6a9fb0fc4cfe5f91e2977bd6'),
    '11': ObjectId('6a9fb0fc4cfe5f91e2977bd7')
  }
}
Atlas atlas-3m3ssv-shard-0 [primary] test> db.students.find([rollNo : 102])
Uncaught:
SyntaxError: Unexpected token, expected "," (1:25)

> 1 | db.students.find([rollNo : 102])
    |                          ^
  2 |

Atlas atlas-3m3ssv-shard-0 [primary] test> db.students.find({rollNo : 102})
[
  {
    _id: ObjectId('6a9fb0fc4cfe5f91e2977bcd'),
    rollNo: 102,
    name: 'Rahul',
    age: 22,
    department: 'ECE',
    marks: 72,
    skills: [ 'C', 'Python', 'Arduino' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: false
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] test> use Student
switched to db Student
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.insertMany([
|     {
|         rollNo: 101,
|         name: "Vasanth",
|         age: 21,
|         department: "CSE",
|         marks: 85,
|         skills: ["Java", "Python", "MongoDB"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 102,
|         name: "Rahul",
|         age: 22,
|         department: "ECE",
|         marks: 72,
|         skills: ["C", "Python", "Arduino"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 103,
|         name: "Priya",
|         age: 20,
|         department: "CSE",
|         marks: 91,
|         skills: ["Java", "Python", "AI"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 104,
|         name: "Arjun",
|         age: 23,
|         department: "MECH",
|         marks: 68,
|         skills: ["AutoCAD", "C", "Java"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         }
|     },
|
|     {
|         rollNo: 105,
|         name: "Sneha",
|         age: 21,
|         department: "IT",
|         marks: 88,
|         skills: ["Python", "MongoDB", "HTML"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 106,
|         name: "Kiran",
|         age: 24,
|         department: "EEE",
|         marks: 65,
|         skills: ["C", "Arduino", "MATLAB"],
|         address: {
|             city: "Pune",
|             state: "Maharashtra"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 107,
|         name: "Anjali",
|         age: 20,
|         department: "CSE",
|         marks: 95,
|         skills: ["Java", "Python", "AI", "MongoDB"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 108,
|         name: "Rohit",
|         age: 22,
|         department: "IT",
|         marks: 76,
|         skills: ["JavaScript", "HTML", "CSS"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 109,
|         name: "Divya",
|         age: 21,
|         department: "CSE",
|         marks: 89,
|         skills: ["Python", "MongoDB", "Java"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 110,
|         name: "Suresh",
|         age: 23,
|         department: "CIVIL",
|         marks: 70,
|         skills: ["AutoCAD", "C", "STAAD"],
|         address: {
|             city: "Vijayawada",
|             state: "Andhra Pradesh"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 111,
|         name: "Meena",
|         age: 22,
|         department: "ECE",
|         marks: 82,
|         skills: ["Python", "Arduino", "IoT"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 112,
|         name: "Akash",
|         age: 25,
|         department: "CSE",
|         marks: 60,
|         skills: ["C", "Java"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         },
|         scholarship: false
|     }
| ])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6a9fb3a14cfe5f91e2977bd8'),
    '1': ObjectId('6a9fb3a14cfe5f91e2977bd9'),
    '2': ObjectId('6a9fb3a14cfe5f91e2977bda'),
    '3': ObjectId('6a9fb3a14cfe5f91e2977bdb'),
    '4': ObjectId('6a9fb3a14cfe5f91e2977bdc'),
    '5': ObjectId('6a9fb3a14cfe5f91e2977bdd'),
    '6': ObjectId('6a9fb3a14cfe5f91e2977bde'),
    '7': ObjectId('6a9fb3a14cfe5f91e2977bdf'),
    '8': ObjectId('6a9fb3a14cfe5f91e2977be0'),
    '9': ObjectId('6a9fb3a14cfe5f91e2977be1'),
    '10': ObjectId('6a9fb3a14cfe5f91e2977be2'),
    '11': ObjectId('6a9fb3a14cfe5f91e2977be3')
  }
}
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.deleteMany({})
{ acknowledged: true, deletedCount: 27 }
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.insertMany([
|     {
|         rollNo: 101,
|         name: "Vasanth",
|         age: 21,
|         department: "CSE",
|         marks: 85,
|         skills: ["Java", "Python", "MongoDB"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 102,
|         name: "Rahul",
|         age: 22,
|         department: "ECE",
|         marks: 72,
|         skills: ["C", "Python", "Arduino"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 103,
|         name: "Priya",
|         age: 20,
|         department: "CSE",
|         marks: 91,
|         skills: ["Java", "Python", "AI"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 104,
|         name: "Arjun",
|         age: 23,
|         department: "MECH",
|         marks: 68,
|         skills: ["AutoCAD", "C", "Java"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         }
|     },
|
|     {
|         rollNo: 105,
|         name: "Sneha",
|         age: 21,
|         department: "IT",
|         marks: 88,
|         skills: ["Python", "MongoDB", "HTML"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 106,
|         name: "Kiran",
|         age: 24,
|         department: "EEE",
|         marks: 65,
|         skills: ["C", "Arduino", "MATLAB"],
|         address: {
|             city: "Pune",
|             state: "Maharashtra"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 107,
|         name: "Anjali",
|         age: 20,
|         department: "CSE",
|         marks: 95,
|         skills: ["Java", "Python", "AI", "MongoDB"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 108,
|         name: "Rohit",
|         age: 22,
|         department: "IT",
|         marks: 76,
|         skills: ["JavaScript", "HTML", "CSS"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 109,
|         name: "Divya",
|         age: 21,
|         department: "CSE",
|         marks: 89,
|         skills: ["Python", "MongoDB", "Java"],
|         address: {
|             city: "Chennai",
|             state: "Tamil Nadu"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 110,
|         name: "Suresh",
|         age: 23,
|         department: "CIVIL",
|         marks: 70,
|         skills: ["AutoCAD", "C", "STAAD"],
|         address: {
|             city: "Vijayawada",
|             state: "Andhra Pradesh"
|         },
|         scholarship: false
|     },
|
|     {
|         rollNo: 111,
|         name: "Meena",
|         age: 22,
|         department: "ECE",
|         marks: 82,
|         skills: ["Python", "Arduino", "IoT"],
|         address: {
|             city: "Bangalore",
|             state: "Karnataka"
|         },
|         scholarship: true
|     },
|
|     {
|         rollNo: 112,
|         name: "Akash",
|         age: 25,
|         department: "CSE",
|         marks: 60,
|         skills: ["C", "Java"],
|         address: {
|             city: "Hyderabad",
|             state: "Telangana"
|         },
|         scholarship: false
|     }
| ])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6a9fb4354cfe5f91e2977be4'),
    '1': ObjectId('6a9fb4354cfe5f91e2977be5'),
    '2': ObjectId('6a9fb4354cfe5f91e2977be6'),
    '3': ObjectId('6a9fb4354cfe5f91e2977be7'),
    '4': ObjectId('6a9fb4354cfe5f91e2977be8'),
    '5': ObjectId('6a9fb4354cfe5f91e2977be9'),
    '6': ObjectId('6a9fb4354cfe5f91e2977bea'),
    '7': ObjectId('6a9fb4354cfe5f91e2977beb'),
    '8': ObjectId('6a9fb4354cfe5f91e2977bec'),
    '9': ObjectId('6a9fb4354cfe5f91e2977bed'),
    '10': ObjectId('6a9fb4354cfe5f91e2977bee'),
    '11': ObjectId('6a9fb4354cfe5f91e2977bef')
  }
}
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({department : {$eq : "CSE"} })
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be4'),
    rollNo: 101,
    name: 'Vasanth',
    age: 21,
    department: 'CSE',
    marks: 85,
    skills: [ 'Java', 'Python', 'MongoDB' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be6'),
    rollNo: 103,
    name: 'Priya',
    age: 20,
    department: 'CSE',
    marks: 91,
    skills: [ 'Java', 'Python', 'AI' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bea'),
    rollNo: 107,
    name: 'Anjali',
    age: 20,
    department: 'CSE',
    marks: 95,
    skills: [ 'Java', 'Python', 'AI', 'MongoDB' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bec'),
    rollNo: 109,
    name: 'Divya',
    age: 21,
    department: 'CSE',
    marks: 89,
    skills: [ 'Python', 'MongoDB', 'Java' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bef'),
    rollNo: 112,
    name: 'Akash',
    age: 25,
    department: 'CSE',
    marks: 60,
    skills: [ 'C', 'Java' ],
    address: { city: 'Hyderabad', state: 'Telangana' },
    scholarship: false
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({marks : {$gt : 70} })
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be4'),
    rollNo: 101,
    name: 'Vasanth',
    age: 21,
    department: 'CSE',
    marks: 85,
    skills: [ 'Java', 'Python', 'MongoDB' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be5'),
    rollNo: 102,
    name: 'Rahul',
    age: 22,
    department: 'ECE',
    marks: 72,
    skills: [ 'C', 'Python', 'Arduino' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be6'),
    rollNo: 103,
    name: 'Priya',
    age: 20,
    department: 'CSE',
    marks: 91,
    skills: [ 'Java', 'Python', 'AI' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be8'),
    rollNo: 105,
    name: 'Sneha',
    age: 21,
    department: 'IT',
    marks: 88,
    skills: [ 'Python', 'MongoDB', 'HTML' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bea'),
    rollNo: 107,
    name: 'Anjali',
    age: 20,
    department: 'CSE',
    marks: 95,
    skills: [ 'Java', 'Python', 'AI', 'MongoDB' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977beb'),
    rollNo: 108,
    name: 'Rohit',
    age: 22,
    department: 'IT',
    marks: 76,
    skills: [ 'JavaScript', 'HTML', 'CSS' ],
    address: { city: 'Hyderabad', state: 'Telangana' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bec'),
    rollNo: 109,
    name: 'Divya',
    age: 21,
    department: 'CSE',
    marks: 89,
    skills: [ 'Python', 'MongoDB', 'Java' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bee'),
    rollNo: 111,
    name: 'Meena',
    age: 22,
    department: 'ECE',
    marks: 82,
    skills: [ 'Python', 'Arduino', 'IoT' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({marks : {$lt : 70} })
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be7'),
    rollNo: 104,
    name: 'Arjun',
    age: 23,
    department: 'MECH',
    marks: 68,
    skills: [ 'AutoCAD', 'C', 'Java' ],
    address: { city: 'Hyderabad', state: 'Telangana' }
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be9'),
    rollNo: 106,
    name: 'Kiran',
    age: 24,
    department: 'EEE',
    marks: 65,
    skills: [ 'C', 'Arduino', 'MATLAB' ],
    address: { city: 'Pune', state: 'Maharashtra' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bef'),
    rollNo: 112,
    name: 'Akash',
    age: 25,
    department: 'CSE',
    marks: 60,
    skills: [ 'C', 'Java' ],
    address: { city: 'Hyderabad', state: 'Telangana' },
    scholarship: false
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({department : {$ne : "EEE"} })
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be4'),
    rollNo: 101,
    name: 'Vasanth',
    age: 21,
    department: 'CSE',
    marks: 85,
    skills: [ 'Java', 'Python', 'MongoDB' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be5'),
    rollNo: 102,
    name: 'Rahul',
    age: 22,
    department: 'ECE',
    marks: 72,
    skills: [ 'C', 'Python', 'Arduino' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be6'),
    rollNo: 103,
    name: 'Priya',
    age: 20,
    department: 'CSE',
    marks: 91,
    skills: [ 'Java', 'Python', 'AI' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be7'),
    rollNo: 104,
    name: 'Arjun',
    age: 23,
    department: 'MECH',
    marks: 68,
    skills: [ 'AutoCAD', 'C', 'Java' ],
    address: { city: 'Hyderabad', state: 'Telangana' }
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be8'),
    rollNo: 105,
    name: 'Sneha',
    age: 21,
    department: 'IT',
    marks: 88,
    skills: [ 'Python', 'MongoDB', 'HTML' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bea'),
    rollNo: 107,
    name: 'Anjali',
    age: 20,
    department: 'CSE',
    marks: 95,
    skills: [ 'Java', 'Python', 'AI', 'MongoDB' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977beb'),
    rollNo: 108,
    name: 'Rohit',
    age: 22,
    department: 'IT',
    marks: 76,
    skills: [ 'JavaScript', 'HTML', 'CSS' ],
    address: { city: 'Hyderabad', state: 'Telangana' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bec'),
    rollNo: 109,
    name: 'Divya',
    age: 21,
    department: 'CSE',
    marks: 89,
    skills: [ 'Python', 'MongoDB', 'Java' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bed'),
    rollNo: 110,
    name: 'Suresh',
    age: 23,
    department: 'CIVIL',
    marks: 70,
    skills: [ 'AutoCAD', 'C', 'STAAD' ],
    address: { city: 'Vijayawada', state: 'Andhra Pradesh' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bee'),
    rollNo: 111,
    name: 'Meena',
    age: 22,
    department: 'ECE',
    marks: 82,
    skills: [ 'Python', 'Arduino', 'IoT' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bef'),
    rollNo: 112,
    name: 'Akash',
    age: 25,
    department: 'CSE',
    marks: 60,
    skills: [ 'C', 'Java' ],
    address: { city: 'Hyderabad', state: 'Telangana' },
    scholarship: false
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({
|     skills: {
|         $all: ["Python", "MongoDB"]
|     }
| })
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be4'),
    rollNo: 101,
    name: 'Vasanth',
    age: 21,
    department: 'CSE',
    marks: 85,
    skills: [ 'Java', 'Python', 'MongoDB' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be8'),
    rollNo: 105,
    name: 'Sneha',
    age: 21,
    department: 'IT',
    marks: 88,
    skills: [ 'Python', 'MongoDB', 'HTML' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bea'),
    rollNo: 107,
    name: 'Anjali',
    age: 20,
    department: 'CSE',
    marks: 95,
    skills: [ 'Java', 'Python', 'AI', 'MongoDB' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bec'),
    rollNo: 109,
    name: 'Divya',
    age: 21,
    department: 'CSE',
    marks: 89,
    skills: [ 'Python', 'MongoDB', 'Java' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({
|     skills: {
|         $all: ["Python", "MongoDB"]
|     }
| })
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be4'),
    rollNo: 101,
    name: 'Vasanth',
    age: 21,
    department: 'CSE',
    marks: 85,
    skills: [ 'Java', 'Python', 'MongoDB' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be8'),
    rollNo: 105,
    name: 'Sneha',
    age: 21,
    department: 'IT',
    marks: 88,
    skills: [ 'Python', 'MongoDB', 'HTML' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bea'),
    rollNo: 107,
    name: 'Anjali',
    age: 20,
    department: 'CSE',
    marks: 95,
    skills: [ 'Java', 'Python', 'AI', 'MongoDB' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bec'),
    rollNo: 109,
    name: 'Divya',
    age: 21,
    department: 'CSE',
    marks: 89,
    skills: [ 'Python', 'MongoDB', 'Java' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({ scholarship : { $exists : false}})
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be7'),
    rollNo: 104,
    name: 'Arjun',
    age: 23,
    department: 'MECH',
    marks: 68,
    skills: [ 'AutoCAD', 'C', 'Java' ],
    address: { city: 'Hyderabad', state: 'Telangana' }
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student> db.students.find({ scholarship : { $exists : true}})
[
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be4'),
    rollNo: 101,
    name: 'Vasanth',
    age: 21,
    department: 'CSE',
    marks: 85,
    skills: [ 'Java', 'Python', 'MongoDB' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be5'),
    rollNo: 102,
    name: 'Rahul',
    age: 22,
    department: 'ECE',
    marks: 72,
    skills: [ 'C', 'Python', 'Arduino' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be6'),
    rollNo: 103,
    name: 'Priya',
    age: 20,
    department: 'CSE',
    marks: 91,
    skills: [ 'Java', 'Python', 'AI' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be8'),
    rollNo: 105,
    name: 'Sneha',
    age: 21,
    department: 'IT',
    marks: 88,
    skills: [ 'Python', 'MongoDB', 'HTML' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977be9'),
    rollNo: 106,
    name: 'Kiran',
    age: 24,
    department: 'EEE',
    marks: 65,
    skills: [ 'C', 'Arduino', 'MATLAB' ],
    address: { city: 'Pune', state: 'Maharashtra' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bea'),
    rollNo: 107,
    name: 'Anjali',
    age: 20,
    department: 'CSE',
    marks: 95,
    skills: [ 'Java', 'Python', 'AI', 'MongoDB' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977beb'),
    rollNo: 108,
    name: 'Rohit',
    age: 22,
    department: 'IT',
    marks: 76,
    skills: [ 'JavaScript', 'HTML', 'CSS' ],
    address: { city: 'Hyderabad', state: 'Telangana' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bec'),
    rollNo: 109,
    name: 'Divya',
    age: 21,
    department: 'CSE',
    marks: 89,
    skills: [ 'Python', 'MongoDB', 'Java' ],
    address: { city: 'Chennai', state: 'Tamil Nadu' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bed'),
    rollNo: 110,
    name: 'Suresh',
    age: 23,
    department: 'CIVIL',
    marks: 70,
    skills: [ 'AutoCAD', 'C', 'STAAD' ],
    address: { city: 'Vijayawada', state: 'Andhra Pradesh' },
    scholarship: false
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bee'),
    rollNo: 111,
    name: 'Meena',
    age: 22,
    department: 'ECE',
    marks: 82,
    skills: [ 'Python', 'Arduino', 'IoT' ],
    address: { city: 'Bangalore', state: 'Karnataka' },
    scholarship: true
  },
  {
    _id: ObjectId('6a9fb4354cfe5f91e2977bef'),
    rollNo: 112,
    name: 'Akash',
    age: 25,
    department: 'CSE',
    marks: 60,
    skills: [ 'C', 'Java' ],
    address: { city: 'Hyderabad', state: 'Telangana' },
    scholarship: false
  }
]
Atlas atlas-3m3ssv-shard-0 [primary] Student>
