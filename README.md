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
##### or
    
    function checkPalindrome(string) {
    
        // convert string to an array
        const arrayValues = string.split('');
    
        // reverse the array values
        const reverseArrayValues = arrayValues.reverse();
    
        // convert array to string
        const reverseString = reverseArrayValues.join('');
    
        if(string == reverseString) {
            console.log('It is a palindrome');
        }
        else {
            console.log('It is not a palindrome');
        }
    }
    
        //take input
        const string = prompt('Enter a string: ');
        
        checkPalindrome(string);
    
### 4. Write a JavaScript program to reverse a given string
    let str = prompt("Enter a string : ");
    let new_str=""
    for(let i = str.length-1;i>=0;i--){
        new_str+=str[i];
        
    }
    
    console.log(new_str);
### 5. Write a JavaScript function that takes an array of numbers and returns a new array with only the even numbers. 
    const arr = [23,24,25,26,27,28,32,33,34];

    let new_arr = arr.filter(function even(val){
            return val%2===0;
        })
    console.log(new_arr);

