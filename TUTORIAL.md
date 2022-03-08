# Filter and Find
```javascript
// Filter and Find
// Filter - returns a new array, can manipulate the size of new array (unlike map), returns based on condition
// Find - returns single instance, returns first match, if no match - undefined
const people = [
  { name: 'bob', age: 20, position: 'developer' },
  { name: 'peter', age: 25, position: 'designer' },
  { name: 'susy', age: 30, position: 'the boss' },
  { name: 'anna', age: 35, position: 'intern' },
];


/*
##
const emptyResponsePrintOnly=people.filter(p=>console.log(p));
O/P
{ name: 'bob', age: 20, position: 'developer' }
{ name: 'peter', age: 25, position: 'designer' }
{ name: 'susy', age: 30, position: 'the boss' }
{ name: 'anna', age: 35, position: 'intern' }


##
console.log(emptyResponsePrintOnly);
O/P
[]


##
const returnSomething=people.filter((p)=>{return true});
console.log(returnSomething);
O/P
[ { name: 'bob', age: 20, position: 'developer' },
  { name: 'peter', age: 25, position: 'designer' },
  { name: 'susy', age: 30, position: 'the boss' },
  { name: 'anna', age: 35, position: 'intern' } ]


##
const emptyWithFalse=people.filter((p)=>{return false});
console.log(emptyWithFalse);
O/P
[]


##
const youngerPeople=people.filter((p)=>{
                           if(p.age<30){
                                return true;
                            }
                    });
console.log(youngerPeople);
O/P
[ { name: 'bob', age: 20, position: 'developer' },
  { name: 'peter', age: 25, position: 'designer' } ]
  
  
##
const youngerPeople2=people.filter((p)=> {
    return p.age<30
    
});
console.log(youngerPeople2);
O/P
[ { name: 'bob', age: 20, position: 'developer' },
  { name: 'peter', age: 25, position: 'designer' } ]


##
const developersOnly=people.filter(p=>p.position==='developer');
console.log(developersOnly);
O/P
[ { name: 'bob', age: 20, position: 'developer' } ]


##
const unknownPositionFilter=people.filter(p=>p.position==='account');
console.log(unknownPositionFilter);
O/P
[]


##
const singleDeveloperMatch=people.find(p=>p.position==='developer');
console.log(singleDeveloperMatch);
O/P
{ name: 'bob', age: 20, position: 'developer' }


##
const multipleMatchFind=people.find(p=>p.age>20);
console.log(multipleMatchFind);
O/P
{ name: 'peter', age: 25, position: 'designer' }


##
const noMatchUsingFind=people.find(p=>p.position==='account');
console.log(noMatchUsingFind);
O/P
undefined

*/

```
