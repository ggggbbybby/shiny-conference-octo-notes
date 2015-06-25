### Event Emitters
 
listen + broadcast with `on` and `emit`

```
ref = new Firebase('url')
//ref.on('value', console.log.bind(console)); // on value changes, print debug
//ref.off('value') // turn off callbacks on this particular event

// callbacks
function onDataChange (snapshot) {
  console.log('click!', snapshot.val()); // dump the changed object tree
}

function onChildChange (snapshot) {
  console.log(snapshot.key(), snapshot.val()) // dump the changed child and its new value
}

ref.on('value', onDataChange) // watches for data changes on the entire object, dumps the whole object
ref.on('child_added', onChildChange) // dumps the key changed 
// other events: 'child_changed', 'child_deleted'
ref.child('temperature').on('value', onDataChange) // watch for data changes just on the 'temperature' object 


// NB Empty Nodes are null and get cleaned up immediately. No orphaned objects in your data. 
ref.set({foo: {bar: null}}) // nothing happens



// Destructive Writes with set
ref.set('foo')
ref.set( {foo: 'bar'})

// Merge-y Writes, overwrites baz if it exists, adds it if it doesn't 
ref.update( {baz: 'qux'})

// Writing to Children
ref.child('foo').set('bar') // by name
ref.child('foo/bar/baz/qux').set('hello world'); // by path


// Arrays + Concurrency
ref.child('numbers').set(['uno', 'dos', 'tres']);
ref.child('numbers/4').set('quatro'); // not safe -- what if somebody else is also writing to the last element of this array?
ref.child('numbers').push('quatro') // safe, will do concurrent pushes in order (w/ some tie-breaking randomness)




```
