---
title: "JSON Generator – tool for generating random JSON data"
source: "https://app.json-generator.com/E8QIJ321co7I"
author:
  - "[[Vazha Omanashvili]]"
published:
created: 2025-08-29
description: "A JSON data generator. JSON Generator generates data according to the template and saves it. Data can be requested from server using ajax with jsonp."
tags:
  - "clippings"
---
```
xxxxxxxxxx
```

1

32

1

```
JG.repeat(5, 10, {
```

2

```
id: JG.objectId(),
```

3

```
email() {
```

4

```
return (
```

5

```
_.snakeCase(this.profile.name) +
```

6

```
'@' +
```

7

```
this.profile.company +
```

8

```
JG.domainZone()
```

9

```
).toLowerCase();
```

10

```
},
```

11

```
username() {
```

12

```
return (_.words(this.profile.name)[0] + moment(this.profile.dob).format('YY')).toLowerCase();
```

13

```
},
```

14

```
profile: {
```

15

```
name: \`${JG.firstName()} ${JG.lastName()}\`,
```

16

```
company: JG.company(),
```

17

```
dob: moment(JG.date(new Date(1988, 0, 1), new Date(1995, 0, 1))).format('YYYY-MM-DD'),
```

18

```
address: \`${JG.integer(1, 100)} ${JG.street()}, ${JG.city()}, ${JG.state()}\`,
```

19

```
location: {
```

20

```
lat: JG.floating(-90, 90, 6),
```

21

```
long: JG.floating(-180, 180, 6),
```

22

```
},
```

23

```
about: JG.loremIpsum({ units: 'sentences', count: 2 }),
```

24

```
},
```

25

```
apiKey: JG.guid(),
```

26

```
roles: _.uniq(JG.repeat(2, JG.random('owner', 'admin', 'member', 'guest'))),
```

27

```
createdAt: JG.date(new Date(2010, 0, 1), new Date(2015, 0, 1)),
```

28

```
updatedAt() {
```

29

```
return moment(this.createdAt).add(1, 'days');
```

30

```
},
```

31

```
});
```

32

```
​
```

```
xxxxxxxxxx
```

1

229

1

```
[
```

2

```
{
```

3

```
"id": "68b1b329623ab258fa1f6bd1",
```

4

```
"email": "larson_forbes@yogasm.show",
```

5

```
"roles": [
```

6

```
"member"
```

7

```
],
```

8

```
"apiKey": "3a6503ef-c1d7-4f40-8095-398dc946eaaf",
```

9

```
"profile": {
```

10

```
"dob": "1993-05-23",
```

11

```
"name": "Larson Forbes",
```

12

```
"about": "Est ea et consectetur minim nisi culpa ex occaecat sit aute eiusmod dolore quis. Occaecat et reprehenderit exercitation culpa ullamco eu deserunt tempor aute in anim.",
```

13

```
"address": "31 Pierrepont Place, Veyo, New Mexico",
```

14

```
"company": "Yogasm",
```

15

```
"location": {
```

16

```
"lat": -58.261258,
```

17

```
"long": 135.688577
```

18

```
}
```

19

```
},
```

20

```
"username": "larson93",
```

21

```
"createdAt": "2014-06-08T02:30:02.791Z",
```

22

```
"updatedAt": "2014-06-09T02:30:02.791Z"
```

23

```
},
```

24

```
{
```

25

```
"id": "68b1b329ee8c8a02bafe21d6",
```

26

```
"email": "sykes_kane@vendblend.vet",
```

27

```
"roles": [
```

28

```
"guest"
```

29

```
],
```

30

```
"apiKey": "378054b5-ff94-4bdf-b1f8-df8fd0ac8fe1",
```

31

```
"profile": {
```

32

```
"dob": "1991-01-23",
```

33

```
"name": "Sykes Kane",
```

34

```
"about": "Minim anim pariatur et ad eu qui deserunt nostrud ex veniam aliqua fugiat culpa. Sint incididunt quis ad voluptate sunt quis magna consectetur labore.",
```

35

```
"address": "19 Joralemon Street, Bowie, West Virginia",
```

36

```
"company": "Vendblend",
```

37

```
"location": {
```

38

```
"lat": 40.962138,
```

39

```
"long": 43.512166
```

40

```
}
```

41

```
},
```

42

```
"username": "sykes91",
```

43

```
"createdAt": "2011-02-05T09:16:39.846Z",
```

44

```
"updatedAt": "2011-02-06T09:16:39.846Z"
```

45

```
},
```

46

```
{
```

47

```
"id": "68b1b329e3c22fc1b3990b78",
```

48

```
"email": "oconnor_lane@cognicode.builders",
```

49

```
"roles": [
```

50

```
"admin",
```

51

```
"owner"
```

52

```
],
```

53

```
"apiKey": "2d0053c7-9bd7-4a15-92f1-e12a101c960d",
```

54

```
"profile": {
```

55

```
"dob": "1992-11-23",
```

56

```
"name": "Oconnor Lane",
```

57

```
"about": "Do ea officia excepteur dolor duis nulla proident velit voluptate in eiusmod incididunt. Incididunt labore voluptate ullamco quis excepteur veniam duis consectetur Lorem Lorem aliqua.",
```

58

```
"address": "80 Stewart Street, Noxen, Nevada",
```

59

```
"company": "Cognicode",
```

60

```
"location": {
```