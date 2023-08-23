# JavaScript-PracticeSet
# JavaScript-PracticeSet

### 1. Write a JavaScript program to find the maximum number in an array. 


    const arr = [23, 34, 54, 670, 85, 63, 96, 123, 348, 273];
    var largest =0;

    arr.forEach(function large(val){
        if(val>=largest){
            largest = val;
            
        }
    })
   ##### or

    const arr = [1, 26, 3, 4, 5, 3, 2];
    var largest=0;
    for(let i=0; i<=arr.length;i++){
            if(arr[i]>largest){
        largest=arr[i];
    }}

    console.log(largest);

### 2.  Write a JavaScript function to check if a given string is a palindrome (reads the same forwards and backwards). 

    const str = prompt("Enter a letter : ")

    function palindrome(val){
        for(let i = 0; i<val.length/2;i++){
            if (val[i] !== val[val.length -1 -i]){
                return "NOT a Palindrome";
                
            }
        }
        return "It is a Palindrome";
    }
    var pal = palindrome(str);

    console.log(pal);


