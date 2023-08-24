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
### 6. Write a JavaScript program to calculate the factorial of a given number. 
    let num = Number(prompt("Enter a number : "));
    
    
    function fact(num){
        if (num==0 || num==1){
            return 1;
        }else{
            return num*=fact(num-1);
        }
    }
    
    console.log(fact(num));
### 7. Write a JavaScript function to check if a given number is prime. 
    const num = Number(prompt("Enter a Number : "));
    let flag =0
    if (num==0 || num==1){
        console.log("Neither Prime nor a composite Number ");
        flag=1;
    }else if(num>1){
        for(i=2;i<num;i++){
            if(num%i===0){
                console.log("A composite number");
                flag=1;
                break;
            }
        }
        
    }
    if(flag===0){
        console.log("It is a prime nummber")
    }
### 8. Write a JavaScript program to find the largest element in a nested array. 
    const arr =[[12,23,21],[67,23,12],[23,34,233]];  
    let largest =0;
    for(let i=0;i<arr.length;i++){
        for(j=0;j<arr[i].length;j++){
            if(arr[i][j]>largest){
                largest=arr[i][j];
            }
        }
    }
    console.log("The largest element in this nested array is ",largest);
### 9. Write a JavaScript function that returns the Fibonacci sequence up to a given number of terms. 
    const m = Number(prompt("Enter a number : "));
    let a=0;
    let b=1;
    
    for(let i=0;i<m;i++){
        if(a==0){
            console.log(a);
        }
        console.log(b);
        c = a+b;
        a=b;
        b=c;
    }
### 10. Write a JavaScript program to convert a string to title case (capitalize the first letter of each word). 
    function capital_letter(str) 
    {
        str = str.split(" ");
    
        for (var i = 0, x = str.length; i < x; i++) {
            str[i] = str[i][0].toUpperCase() + str[i].substr(1);
        }
    
        return str.join(" ");
    }
    
    console.log(capital_letter("shyam pratap singh"));



