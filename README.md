# Mongo-DB-Day-2

## Task - 2

**Q: Find all the topics and tasks which are thought in the month of October**

```javascript
db.data
    .find(
        { users: "student" },
        { attendance: 0, company_drives: 0, users: 0, codekata: 0 }
    )
    .pretty();
```

**Q: Find all the company drives which appeared between 15 oct-2020 and 31-oct-2020**

```javascript
db.data
    .find(
        { users: "student" },
        { attendance: 0, topic: 0, task: 0, users: 0, codekata: 0 }
    )
    .pretty();
```

**Q: Find all the company drives and students who are appeared for the placement**

```javascript
db.data
    .find(
        { users: "student" },
        { attendance: 0, topic: 0, task: 0, users: 0, codekata: 0 }
    )
    .pretty();
```

**Q: Find the number of problems solved by the user in codekata**

```javascript
db.data
    .find(
        { users: "student" },
        { attendance: 0, topic: 0, task: 0, company_drives: 0, users: 0 }
    )
    .pretty();
```

**Q: Find all the mentors with who has the mentee's count more than 15**

```javascript
db.data.find({ mentee_count: { $gt: 15 } }).pretty();
```
