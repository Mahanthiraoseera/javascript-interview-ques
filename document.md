
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
2.1.write a function to check the given string is palindrome? Solution One
```
let a=prompt("Enter a string ");
function checkString(str){
    let l=str.length;
    let reverse=""
    for(let i=0;i<l;i++){
        reverse=str[i]+reverse
    }
    if(a==reverse){
        return `${str} is palindrome`
    }else{
        return `${str} is not a palindrome`
    }
}
console.log(checkString(a))
```
Solution Two
```
let a=prompt("Enter a string ");
function checkString(str){
    let b=(str.split("").reverse().join(""))
    if(a==b){
        return `${str} is palindrome`
    }else{
        return `${str} is not a palindrome`
    }
}
console.log(checkString(a))
```

