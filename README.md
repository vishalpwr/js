# javascript-tricks

## 1
#### String to Array conversion
**ex1**
```
//string to array
const str = 'javascript'
const ar = str.split('')
console.log(ar)
// Output
// ['j','a','v','a','s','c','r','i','p','t']
```
**ex2:**
or using Array's method
```
const ar1 = Array.from(str)
console.log(ar1)
// Output
// ['j','a','v','a','s','c','r','i','p','t']
```
-----------------------------------------------------
## 2
#### Remove duplicate items from array
```
const ar = ['a', 'b', 'c', 'a', 'd', 'e', 'c'];
const set = new Set(ar);
//set returns a object of unique items
const array = [...set];
console.log(array)
// Output
// ['a', 'b', 'c', 'd', 'e'];
```
-----------------------------------------------------
## 3
#### Get total of items
```
const numbersAr = [1,2,3,4,7,8,0]
const total = numbersAr.reduce((a, b) => {
	return a + b;
})
console.log(total)
// Output:
// 25
```
-----------------------------------------------------
## 4
### Merge 2 Arrays
```
const a=[1,2,3,4];
const b=[5,6,7,8];
const c=[...a, ...b];
console.log(c)
// Output:
// [1,2,3,4,5,6,7,8]
```
-----------------------------------------------------
## 5
#### The splice() method adds and/or removes array elements. The splice() method overwrites the original array
**ex1**
```
const ar=[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16];
ar.splice(1, 0, 'c', 'd')
// splice(index, howmany, item)
console.log(ar);
// Output:
// [ 1, 'c', 'd', 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16 ]
```
**ex2**
```
ar.splice(1, 2, 'e', 'f')
// splice(index, howmany, item)
console.log(ar);
// Output:
// [ 1, 'c', 'd', 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16 ]

```
-----------------------------------------------------
