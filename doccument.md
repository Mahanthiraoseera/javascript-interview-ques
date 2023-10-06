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
