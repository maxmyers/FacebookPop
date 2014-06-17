FacebookPop


## 5 Steps For Facebook Pop



## Arrays

```js
// Array
var shoppingList = ["catfish", "water", "lemons"]
shoppingList[1] = "bottle of water"               // update 
shoppingList.count                                // size of array (3)
shoppingList.append("eggs")
shoppingList += "Milk"

// Array slicing
var fibList = [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 5]
fibList[4..6] // [3, 5]. Note: the end range value is exclusive
fibList[1..fibList.endIndex] // all except first item
// Subscripting returns the Slice type, instead of the Array type.
// You may need to cast it to Array in order to satisfy the type checker
Array(fibList[0..4])

// Variants of creating an array. All three are equivalent.
var emptyArray1 = String[]()
var emptyArray2: String[] = []
var emptyArray3: String[] = String[]()
```

