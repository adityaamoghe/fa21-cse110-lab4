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

- b) Output: \
        Explanation:
        
- c) Output: \
        Explanation:
        
- d) Output: \
        Explanation:
        
- e) Output: \
        Explanation:
        
- f) Output: \
        Explanation:
        
- g) Output: \
        Explanation:
        
- h) Output: \
        Explanation:
        