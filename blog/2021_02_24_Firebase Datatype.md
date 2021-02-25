# Firestore Reference Datatype

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

### Adding reference
---
In order to add Document Path,

```ts
firebase.firestore().collection("collection").add({property: firebase.firestore().doc(`/properties/${propertyId}`)})
```

