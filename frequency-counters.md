# Frequency Counters

**This method can often avoid having to use nested loops with arrays and strings**

Pattern that uses JS objects or sets to collect values or the frequency of values 

Good to use when you have multiplee pieces of data and you have to compare them to see if they have simmilar values

- anograms 
- value inside of another value
- comparing two or more inputs of data


The idea: 
Loop over each array one time individually instead of nesting them utilizing an object.

## write it out

create an edge case that if the length of the two values being compared do not match, the return is false
create two variables that equal two empty objects to count the individuual frequencies in the arrays
create a for (or for of) loop that will take eeach value of array 1 and add one to the frequency counter if it's already in there
or initialize it to one if it is not in there.
Repeat the same for of loop for the second array and frequency counter 


**at this point, you will have two objects that identify the items in the array and how many times they occur in that array**

From there, you're going to loop through the first object by utilizing a for..in loop 

This for in loop will look at each key in the object and see if that key is in the second object created

  If that key is not in the second object - return false

  if it is in the second object, 
  check to see if the valess of the keys are the same
  
  do this by taking the second frequency counter with its key and seeing if it does not equal the first frequency counter and it's key
  
  if that statement is true than return false .
  
  
If this whole loop runs and you get out of the loop, return true 



