1. At line 12, 3 will be printed. This is because the prices.length is 3 (because there are 3 numbers in the array), and so i will keep adding 1 until it equals prices.length, which ends the for loop and then prints i. There is no block scoping issues as the variable is not being randomly updated outside the for loop. Because var can be used globally, it can still be printed/ used outside the for loop.
2. At line 12, 150 will be printed. The variable discountedPrice will be updated under the for loop. Looping through the for loop, as it accesses the last index in the array, which is number 300, discountedPrice will be updated to 150 (computed from prices[i] * (1-discount)). Initalizing var discountedPrice does not cause an error and will still update the variable. Because var can be used globally, it can still be printed/ used outside the for loop.
3. At line 14, 150 will be printed. finalPrice is calculated after calculating the discountedPrice. The variable discountedPrice does not lead to an error, and nor does finalPrice print something else that isn't supposed to be 150 (150 is expted). The variable is not being updated outside of the for loop so block scoping isn't an issue and it'll get the expected 150. Because var can be used globally, it can still be printed/ used outside the for loop.
4. The function returns [50, 100, 150]. Within the for loop, it loops 3 times. During every loop, it grabs the prices array index & calculate the discountedPrice, then calculates the finalPrice, and pushes the finalPice in the discounted array, essentially adding it. discountedPruce & finalPrice computes the calculations correctly and is not affected from block-scoping (not being used outside of the for loop), discounted also is okay and is not affected from block scoping as well. Therefore, discounted returned will be what is expected. Because var can be used globally, it can still be used to return.
5. The code causes a ReferenceError because i is not defined. Because i is defined in the for loop, this means that i can only be used in the for loop (a rule for using let), nowhere else outside the for loop (unless it is initialized outside the for loop). 
6. The code causes a ReferenceError because discountedPrice is not defined. Because discountedPrice is defined in the for loop, this means that discountedPrice can only be used in the for loop (a rule for using let), nowhere else outside the for loop (unless it is initialized outside the for loop).
7. At line 14, it will print 150. The finalPrice variable is initialized in the function, so finalPrice can be used in the for loop and outside of the for loop within the function.
8. The function will return [50, 100, 150]. The variable i and variable discountedPrice is initialized inside the for loop and is only used in the for loop so it will work as it's supposed to, the variables discounted and finalPrice is initialized within the function (outside the for loop) and will work throughout the function so it'll work as is, therefore discounted will return the expected.
9. The code causes a ReferenceError because i is not defined. Because i is defined in the for loop, this means that i can only be used in the for loop (a rule for using let), nowhere else outside the for loop (unless it is initialized outside the for loop). 
10. At line 12, it will print 3. The length of prices is 3. Length is not being assigned anywhere else, only when it's being initalized, so it will print 3 and print 3 always.
11. The function will return [50, 100, 150] as expected. There are no assignings to the const variables (aside from initialization) so everything will work as is. The i variable works as is because it's only being used in the for loop as it's supposted to. The variable discountedPrice will work because it is initializing to a new variable (a const declaration) and it's not re-assigning the variable.
12. 
<ol type="A">
    <li>student.name</li>
    <li>student['Grad Year']</li>
    <li>student.greeting()</li>
    <li>student['Favorite Teacher'].name</li>
    <li>student.courseLoad[0]</li>
</ol>
13.
<ol type="A">
    <li>'32' because integers are able to make to their string representation with concatenation. </li>
    <li>1 because it is subtraction and only used for numbers, so it'll concert '3' to 3.</li>
    <li>3 because addition with a null will convert it to 0 (now in numerical context)</li>
    <li>'3null' because in this context this is string concatenation with '3' so it'll convert null to 'null'</li>
    <li>4 because addition with an integer so true becomes integer 1.</li>
    <li>0 because false and null are not strings, and because of addition it'll make both to the integer 0</li>
    <li>'3undefined' because '3' is string so it'll be concatenation due to addition, so undefined turns into string </li>
    <li>Nan because of subtraction, '3' and undefined must be converted to a number, however, undefined cannot be converted to a number so NaN.</li>
</ol>
14.
<ol type = "A">
    <li>True because string'2' becomes number 2</li>
    <li>False because dictionary comparison. First char '2' is greater than first char '1'.</li>
    <li>True because '2' is converted to integer 2 then compared.</li>
    <li>False because different types (integer & string).</li>
    <li>False because true is converted to 1 and then compared to 2.</li>
    <li>True because converting 2 is true & is equal to each other without type coercion.</li>
</ol>
15. == converts types to match & compares the value only. === compares both value and type and does not do conversion.
17. The result is [2, 4, 6]. A function is a value. In modifyArray, the first parameter is [1,2,3] and the second parameter is doSomething. doSomething(num) is essentially a value. modifyArray will access the newArr & push in the returned value from calling doSomething (which is the input number * 2). After the for loop, newArr will be returned [2,4,6] as expected.
19. 
1
4
3
2
