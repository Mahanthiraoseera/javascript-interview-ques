
1.write a function to reverse the string?
Solution One
```
let a=prompt("Enter a string ")
function reverseString(str){
    let l=str.length;
    let reverse=""
    for(let i=0;i<l;i++){
        reverse=str[i]+reverse
    }
    return reverse
}
console.log(reverseString(a))
```
Solution two
```
let a=prompt("Enter a string ");
function reverseString(str){
    return str.split("").reverse().join("")
}
console.log(reverseString(a))
```


