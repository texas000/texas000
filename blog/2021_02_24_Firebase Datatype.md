# Firestore Reference Datatype

![Firebase Image](https://www.gstatic.com/devrel-devsite/prod/vf8bcd170103a60a9457e3a7682d3f70251c619395c6349d20b56cd2a80761a19/firebase/images/lockup.png)

There are following datatype in firestore:

- string
- number
- boolean
- map
- array
- null
- timestamp
- geopoint
- reference

### Add reference data

---

In order to add Document Path,

```ts
firebase
	.firestore()
	.collection("collection")
	.add({ property: firebase.firestore().doc(`/properties/${propertyId}`) });
```

### Append Array

---

In order to append Array

```ts
firebase
	.firestore()
	.collection("collection")
	.add({ property: firebase.firestore.FieldValue.arrayUnion(data) });
```

### Adding Number

---

In order to increse number value

```ts
firebase
	.firestore()
	.collection("collection")
	.add({ property: firebase.firestore.FieldValue.increment(1) });
```

### Adding Current Timestamp

---

In order to add server time data

```ts
firebase
	.firestore()
	.collection("collection")
	.add({ property: firebase.firestore.FieldValue.serverTimestamp() });
```
