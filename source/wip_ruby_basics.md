# Ruby Basics

## Goals
After this exercise, a student will be able to:

* Run ruby files from the command line
* Write programs using basic ruby concepts from previous knowledge and information found in reference material
* Use high level, [acceptance tests](http://www.extremeprogramming.org/rules/functionaltests.html){:target="_blank"} to guide development

## XP practices learned

* Whole Team
* Test First Programming

## Tech skill learned

* Ruby language constructs
* Running acceptance tests from the command line
* Running code using irb to try things out
* Running code from a file at the command line

## Resources

**Warning: Some of the online material may not be compatible with your version of Ruby but it is free.**

* Online Materials
    * [Learn to Program Website](http://pine.fm/LearnToProgram/){:target="_blank"}
    * [Learn Ruby the Hard Way](http://ruby.learncodethehardway.org/){:target="_blank"} - when you read "function" substitute the word "method"
    * [Ruby Essentials](http://www.techotopia.com/index.php/Ruby_Essentials){:target="_blank"}
    * [Pickaxe Book](http://ruby-doc.com/docs/ProgrammingRuby/){:target="_blank"}
    * [Ruby Language Documentation page](https://www.ruby-lang.org/en/documentation/){:target="_blank"} - a list of of other references

* Ebooks/Physical Books for Purchase
    * [Learn to Program](http://pragprog.com/book/ltp2/learn-to-program){:target="_blank"} - not a complete reference but great for beginners. Suited for reading cover to cover.
    * [Pickaxe Book](http://pragprog.com/book/ruby4/programming-ruby-1-9-2-0){:target="_blank"} - a pretty complete language reference book. Not meant for reading cover to cover.

## Demo

Greetings

1. The program asks a user for their name by printing the prompt "What is your name?".
1. The program prints out the text "Hello [enteredName]!" where [enteredName] is replaced by the
name entered above.

## Homework

Complete assignments below by getting the tests to pass. Step one is to [fork](https://help.github.com/articles/fork-a-repo){:target="_blank"}
the [starting repository](https://github.com/gSchool/ruby_basics){:target="_blank"} into your account and clone the repository to your local machine
into the gSchool working folder. You should then run `bundle` and then `rspec spec` from the cloned directory to see all of the pending specs. If you want to run only the specs
for a specific assignment, you can run `rspec spec/[spec_file_name]`. For example, to run only the Greetings specs from the demo, you would type `rspec spec/greetings_spec.rb`.

You assignment is to use each of the test files to complete the exercises below. Each exercise should be implemented in a file that is named after the title of the item using
proper Ruby file naming conventions. For example, Guessing Game
should be implemented in a file called "guessing_game.rb".

If you get stuck on one, write as much code as you can then write out your logic using comments and
short English phrases for any code that you do not know how to write.
When you are done, push your code back up to GitHub for review.

(Mike's notes in parens)

1. Guessing Game (this one may be tricky because we have to stub random on the tests...let's look for 5 others to see if we need this one. Another option is to give them the code needed to get the random number to start with so we can stub it properly in the tests)
    1. The program calculates a random number between 1 and 10 when it starts and stores it in a variable. (Figure out how to stub random in the tests.)
    1. The program asks the user for a number by printing the prompt "Please enter a number:".
    1. If that number is less than the random number, print out the string "Higher" and asks for another number
    1. If that number is greater than the random number, print out the string "Lower" and asks for another number.
    1. If that number is equal to the random number, print out "Congratulations!" and stop asking for numbers.

2. Deaf Grandma
  1. Whatever you say to grandma(type into the program), she should respond with 'HUH?!, SPEAK UP SONNY!'
  2. She will only respond to you if you shout (type in all capitals)
  3. If you shout, she can hear you, or at least she thinks she can and responds 'NO, NOT SINCE 1938!'
  4. To make your program more believable, have grandma shout a different year each time; maybe any year at random between 1930-1950 (this part is optional, so maybe we won't use it to avoid stubbing random)
  5. You can't stop talking to grandma until you say 'BYE!'

3. Old-School Roman Numerals
  1. The program has a method that when passed an integer between 1 and 3000 (or so) returns a string containing the proper old-school roman numeral.
  2. I = 1, V = 5, X = 10, L = 50, C = 100, D = 500, M = 1000

4. Interactive Baby Dragon
  1. Write a program that lets you enter feed, walk, put to bed, toss, rock commands.
  2. The dragon should be able to know if it is hungry, tired, needs to go, etc.
  3. Remember since you are inputting just strings, you will need some sort of method dispatch, where your program checks which string was entered and then calls the appropriate method.

5. Birthday Helper
  1. Write a program to read in names and birth dates from a text file.
  2. It should then ask you for a name. You type one in.
  3. It tells you when that person's birthday will be and how old they will be.

6. 99 Bottles of Beer
  1. Write a program that calculates that prints out the lyrics to the song starting with 99 bottles all the way until 0 bottles. 