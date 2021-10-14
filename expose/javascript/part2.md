# Part 2 Answers:
1. At line 12 we will output to console the value of variable *i*. In the console we get the output 3 meaning that the for loop has executed 3 times (i=0,1,2) and has exited the loop when i == prices.length = 3. Therefore we see that line 12 will always output the size of our prices array.
2. At line 13, we will output to the console the value of the last element in our prices array with the discout applied to it. We notice that the variable *discountedPrice* is being updated with every iteration of the for-loop. The console will output 150 because that is $300 with the 50% discount applied to it.
3. At line 14, we will output to the console the value 150. Since this is a *var*, we will be constantly updating the variable *finalPrice* through the life cycle of the for-loop. Thus, the 150 comes from the rounding of (150*100)/100 = 150. The 150 comes from using the discounted price to get the final price.
4. This function will return an array of all the discounted prices. The returned array *discounted* will have the respective discounted prices of the array of prices passed into the *discountedPrices* function.  We have declared *var discounted* at line 3, and each time we calculate the final price after the discount has been applied, we push this value into our discounted array effectively updating it over and until we have looped through the given input array of prices.
5. The code will cause an error. This is because we initiatilized our iterator variable *i* with the keyword "let". Since we call *console.log(i)* outside the for-loop where the scope of *i* exists, we get an error message because it thinks that the variable *i* does not even exist.
6. This code will cause an error. This is because we intialized our *discountedPrice*  variable with the keyword "let". Since we call *console.log(discountedPrice)* outside the for-loop where the scope of *discountedPrice* exists, we get an error message because it thinks that the variable *discountedPrice* does not even exist.
7. At line 14, we will output to console the number 150. This 150 is the price after discount being applied to the original price of 300$ passed in. With a discount of 50% it will give the final price of $150. More importantly, we notice that unlike the previous two questions we do not get thrown an error simply because the scope of *finalPrice* is through the entirety of the *discountPrices* function. The keywords "let" and "var" should be interchangeable because they will both provide scope for the entirety of the *discountPrices* function. 
8. This function will return an array of all the discounted prices respective to the prices array passed in after the given discount is applied. Since we declared the *discounted* array at the top (line 3) with the key word "let" and we call return within the same scope, we will not have any problems. Using the given inputs of prices = [100,200,300] and discount = 0.5, we will be returning the value of *discounted = [50,100,150]*.
9. This code will result in an error. This is because we have define the variable *i* by the keyword "let". Since we are calling *console.log(i)* outside of the scope of where *i* exists, we will get an error for our code.
10. This code will run without any errors. We get an output of 3 because that was the size of the input price array. At the beggining of the function, we define the length with a *const*. We simply return this *const* and no errors occur because we never try to modify it.
11. This was an interesting output that I didn't understand at first. My initial intuition was that we would simply return the empty "[]" array when we called the return statement on line 14 because of the "const" keyword used. However after testing this the actual output was the discounted price array [50,100,150]. This goes to show that in javascript, the "const" keyword in front of an array will allow individual array elements can be reassigned but not the whole array.
12. Below are the 5 parts for question 12:
- a) student.name;
- b) student['Grad Year'];
- c) student.greeting();
- d) student['Favorite Teacher'].name;
- e) student.courseLoad[0];
13. Below are the 8 parts for question 13:
- a) Output: '32'
  
        Explanation: Here the output is of type string. We will convert the number 2 into a string and concatenate both strings into the output given above.

- b) Output: 1
  
        Explanation: Here the output is of type number. Since there is a "-" sign, we will convert the string '3' into a number and subtract 2 from it giving us the output above.
        
- c) Output: 3
  
        Explanation: Here the output is of type number. The null will not affect anything to the addition and we will simply add 3 with 0 giving us the output above.
        
- d) Output: '3null'
  
        Explanation: Here the output is of type string. We will convert the null into the string 'null' and concatenate the it at the end of the string '3' giving us the ouput above.
        
- e) Output: 4
  
        Explanation: Here the output is of type number. The true term will be converted into the number 1. Then addition of 1 and 3 will result in the number output of 4 as given above.
        
- f) Output: 0
  
        Explanation: Here the output is of type number. The false term will be converted into the number 0. The null will be represented as number 0 as well. Addition of both gives us the output above.
        
- g) Output: '3undefined"
  
        Explanation: Here the output is of type string. The undefined term will be converted into the string 'undefined'. This will be concatednated at the end of string '3' by the + operator giving us the output shown above.
        
- h) Output: NaN
  
        Explanation: Here we will have undefined numerical results because it is simply not possible to do such calculations to get a definitive number.

14. Below are the 6 parts for question 14:
- a) Output: true
  
        Explanation: Here the output is of type boolean. Here the string '2' becomes a number and we see that the number 2 is greater than 1 giving us the output true.

- b) Output: false 
  
        Explanation: Here the output is of type boolean. Since both values are of type string, we will compare the first character of both of them. Since '2' is not less than '1' we will get the output false.

- c) Output: true
  
        Explanation: Here the output is of type boolean. Here the string '2' will become a number 2. The statement is thus true because 2 is equal to 2.

- d) Output: false
  
        Explanation: Here the output is of type boolean. Since we use the === comparator, we will not do type conversion and we see that the number 2 is not equal to the string '2'.

- e) Output: false
  
        Explanation: Here the output is of type boolean. The true will get converted to the number 1. We know that 1 does not equal to 2 and therefore we get the output false.

- f) Output: true
  
        Explanation: Here the output is of type boolean. The Boolean converter will turn the number 2 into the boolean true. Since true and true are both equal booleans we get the output of true.

15. The == comparator is used for comparing two values but it ignores the datatype of the variable. The === comparator is also used for comparing two values as well but the operator will also check the datatypes of the two. The === will only return true if and only if the datatype and the values are equivalent of the two variables.
    
16. The answer to this question is found in the part2-question16.js file.

17. The result of the given code will be the array: [2,4,6]. We will first start at line 13, where the function *modifyArray* is being called with parameters [1,2,3] which is an array and second parameter *doSomething* which is a function. Next we move into line 1, and we enter the called function *modifyArray*. We will declare a const array that will have its elements be updated by the for loop that follows. We will push into the new array the return value of the function *callback* which is equivalent to the function *doSomething*. We shall go through our input array, iteratively calling *doSomething* which creates our array values doubled.

18. The answer to this question is found in the part2-question18.js file.

        