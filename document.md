
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
2.write a function to check the given string is palindrome? Solution One
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
3.write a function to return longest word in the given string ? Solution One
```
let a="hello, how are doing this javascript problem"
function longestWord(str){
    let words=str.split(" ")
    let longWord=""
    for(let word of words){
        if(word.length>longWord.length){
            longWord=word
        }
    }
    return longWord;
}
console.log(longestWord(a))
```
4.write a function to return number of vowels in the given string ? Solution One
```
let a=(prompt("Enter a string : "));
function vowelCount(str){
   let vowels=["a","e","i","o","u"]
   let count=0
   for(let char of str.toLowerCase()){
       if(vowels.includes(char)){
           count+=1
       }
   }
   return(count)
}
console.log(vowelCount(a))
```
Solution Two
```
let a=parseInt(prompt("Enter a number : "));
function primeNum(x){
    for(let i=2;i<=parseInt(a/2);i++){
        if(x%i==0){
            return `${x} is not a Prime Number`
        }
    }
    return `${x} is a Prime Number`
}
console.log(primeNum(a))
```
5.write a function to check prime number? Solution One
```
let a=parseInt(prompt("Enter a number : "));
function primeNum(x){
    let count=0;
    for(let i=1;i<=parseInt(a/2);i++){
        if(x%i==0){
            count+=1
        }    
    }
    if(count>1){
        return `${x} is not a Prime Number`
    }else{
        return `${x} is a Prime Number`
    }
}
console.log(primeNum(a))
```

6.write a function to find factorial of given number? Solution One
```
let a=parseInt(prompt("Enter a number : "));
function factorial(x){
    let mul=1
    for(let i=1;i<=x;i++){
        mul*=i
    }
    return mul
}
console.log(factorial(a))
```
7.write a function to remove the duplicates in the given array ? Solution One
```
let arr=[1,2,3,4,4,5,6,7,7,8]
function removeDuplicates(array){
    return [...new Set(array)]
}
console.log(removeDuplicates(arr))
```
Solution Two
```
let arr=[1,2,3,4,4,5,6,7,7,8,8,9,0,0,0]
function removeDuplicates(array){
    let result=[]
    let l=array.length
    for(let i=0;i<l;i++){
        if(result.indexOf(array[i])=="-1"){
            result.push(array[i])
        }
    }
    return result;
}
console.log(removeDuplicates(arr))
```
8.write a function to find the largest number in the given array ? Solution One
```
let arr=[1,2,3,4,4,5,6,7,7,8,8,9,15,0,0,0]
function largestNumber(array){
    let large=array[0]
    let l=array.length
    for(let i=0;i<l;i++){
        if(array[i]>large){
            large=array[i]
        }
    }
    return large;
}
console.log(largestNumber(arr))
```
9.write a function to check the given words are anagrams or not in the given strings ? Solution One
```
let a="HEEllo"
let b="oleelh"
function checkAnagrams(strA,strB){
    let x=strA.toLowerCase().split("").sort().join("")
    let y=strB.toLowerCase().split("").sort().join("")
    return x==y;
}
console.log(checkAnagrams(a,b))
```












