TDD String Calculator
=============

I found another TDD Code Kata that I want to do.  This should take no more than an  hour to do but be sure to follow the instructions because the goal is to do this exercise incrementally and learn how to to TDD.  I haven't done very much TDD in my work environment so this is something I want to get better at and even if you are a TDD expert I hope this will be fun for you.

###Task
* Don't read ahead
* Do one task at a time
* Only test for correct inputs.  No need to try and test for invalid inputs for this kata.


###Steps
1. Create a simple String calculator with a method **int Add(string numbers)**
    1. The method can take 0, 1 or 2 numbers, and will return their sum (for an empty string it will return 0) for example **“” or “1” or “1,2”**
    2. Start with the simplest test case of an empty string and move to 1 and two numbers
    3. Remember to solve things as simply as possible so that you force yourself to write tests you did not think about
    4. Remember to refactor after each passing test
2. Allow the Add method to handle an unknown amount of numbers
3. Allow the Add method to handle new lines between numbers (instead of commas).
    1. the following input is ok:  “1\n2,3”  (will equal 6)
    2. the following input is NOT ok:  “1,\n” (not need to prove it - just clarifying)
4. Support different delimiters
    1. to change a delimiter, the beginning of the string will contain a separate line that looks like this:   “//[delimiter]\n[numbers…]” for example “//;\n1;2” should return three where the default delimiter is ‘;’ .
    2. the first line is optional. all existing scenarios should still be supported
5. Calling Add with a negative number will throw an exception “negatives not allowed” - and the negative that was passed.if there are multiple negatives, show all of them in the exception message


###Bonus / Extra Credit
6. Numbers bigger than 1000 should be ignored, so adding 2 + 1001  = 2
7. Delimiters can be of any length with the following format:  “//[delimiter]\n” for example: “//[***]\n1***2***3” should return 6
8. Allow multiple delimiters like this:  “//[delim1][delim2]\n” for example “//[*][%]\n1*2%3” should return 6.
8. Make sure you can also handle multiple delimiters with length longer than one char


###Reference
Thanks to [Roy Osherove's website](http://www.osherove.com) for this [Code Kata](http://osherove.com/tdd-kata-1/).  He has couple of katas on his website and I'm sure we'll use some more of them as we continue to code kata.

### Answer Submission Instructions
1. Fork [this github repository](https://github.com/CentralArkansasCodeKata/TDDStringCalculator).
2. Write your solution to the problem.
3. Commit your solution to the repository.
4. Post a link to your fork as a comment to [this Prime Factors post](http://codekata.co/2013/09/22/tdd-string-calculator/) on [codekata.co](http://codekata.co).
