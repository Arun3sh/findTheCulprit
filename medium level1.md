1. Find the culprit
fix.html

<!DOCTYPE html>
<html>
<body>
 <script>
 //alert( “I’m JavaScript!’); The quotes are not matching.
 alert( "I’m JavaScript!");
 </script>
 Whats the error in this ?
</body>
</html>

2. Find the culprit and invoke the alert
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>  // The Quotes are the culprit.
</body>
</html>

scripts.js

alert(“I’m invoked!”);

3. Explain the below how it works
explain.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

alert("I'm JavaScript!");
alert('Hello') // this line is not having semicolon
alert(`Wor
 ld`)
alert(3 +
1
+ 2); // this is multiple line code and its working

JavaScript has an automatic semicolon insertion feature and this happens behind the scenes.
JavaScript ignores multiple white spaces.

4. Fix the below to alert Guvi geek
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let admin=9, fname=10.5; 
fname = "Guvi";
lname = "geek"
admin = fname+lname;
alert( admin ); // "Guvi geek"

It is fixed

5. Fix the below to alert hello Guvi geek
fix.html
<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>
script.js
let fname=10.5; 
fname = "Guvi";
lname = "geek"
let name = fname+lname;
//alert( 'hello ${name}' ); // have removed $ and added 
alert( 'hello' + name ); // I'm getting a comment as it has been deprecated.

6. Fix the below to alert sum of two numbers
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let a = prompt("First number?");
let b = prompt("Second number?");
//alert(a + b); Variable a and b are taken as a string.
alert(+a + +b); // Here have used intParse() TO Convert string to number.

7. Fix the below to alert sum of two numbers
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let a = prompt("First number?");
let b = prompt("Second number?");
//alert(a + b); Variable a and b are taken as a string. Before that I was getting alert 0. I just deleted a and reentered it and it worked like a string.
alert(+a + +b); // Here have used intParse() TO Convert string to number.

8. If you run the below scritpt you will get “Code is Blasted”

Explain Why the Code is blasted and how to diffuse it and get “Diffused”.

fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

//var a = "2" > "12"; 
var a = "2" < "12"; // Made 2 less than 12 to get it a false. Usually 2 is < 12 but here they are in string so in 12 first letter (i.e) 1 is consider to get compared with 2. Therefore 2<1 is false.
//Don't touch below this
if (a) {
  console.log("Code is Blasted")
}
else
{
  console.log("Diffused") 
}

9. How to get the success in console.

fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let a = prompt("Enter a number?");
//Don't modify any code below this
if (a) {
 console.log( 'OMG it works for any number inc 0' );
}
else
{
 console.log( "Success" );
}

To get success one should enter 0.

10. How to get the correct score in console.
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let value = prompt('How many runs you scored in this ball');
if (+value === 4) {
      console.log("You hit a Four");
} else if (+value === 6) {
      console.log("You hit a Six");
} else {
      console.log("I couldn't figure out");
}

I have just prased the string to number. To get the correct score.

11. Fix the code to welcome the Employee
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let login = 'Employee';
let message = (login == 'Employee') ? :
  'Greetings' :
  'No login' 
console.log(message);

Have removed unwanted expressions.

12. Fix the code to welcome the boss
fix.html
<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>
script.js
// You cant change the value of the msg
let message;
if (null || 2 || undefined )
{
 message = "welcome boss"; // Rempved the let as message has already been declared and we don't want this to to stay within the scope.
}
else
{
 let message = "Go away";
}
  console.log(message);

13. Fix the code to welcome the boss
fix.html
<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let message;
//let lock = 2;
let lock ; //  I have removed the assigned value to get the statement as false.
//Dont change any code below this 
if (null || lock || undefined )
{
  message = "Go away";
}
else
{
 message = "welcome";
}
  console.log(message);

14. Fix the code to welcome the boss
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let message;
let lock; // I have removed the assigned value to get the statement as false.
//Dont change any code below this
if (lock && " " || undefined )
{
  message = "Go away";
}
else
{
 message = "welcome";
}
console.log(message);

15. Change the code to print
3
2
1
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

//You can change only 2 characters
let i = 3;
while (i) {
  //console.log( --i );
console.log( i-- ); // Changed the pre decrement to post decrement.
}

16. Change the code to print 1 to 10 in 4 lines
fix.html
<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

//let num = 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)
//num += 1
//console.log(num)

let num = 1
for(let i =1; i<=10; i++,num++){
  console.log(num);
}

17. Change the code to print even numbers
fix.html
<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js
//You are allowed to modify only one character 
/* for (let num = 2; num <= 20; num += 1) {
  console.log(num)
}*/

for (let num = 2; num <= 20; num += 1) {
  if(num%2 ==0){
    console.log(num)
  }
}
Added a if statemnt.

18. Change the code to print all the gifts
fix.html
<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let gifts = ["teddy bear", "drone", "doll"];
for (let i = 0; i < 3; i++) {
  console.log('Wrapped ${' + gifts[i] + '} and added a bow!'); // Have added + between the strings and the variable gifts.
}

19. Fix the code to disarm the bomb.
fix.html

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

script.js

let countdown = 100;
//while (countdown > 0) {
while (countdown < 0) { // Have made the expression in a way that it fails. If the condition fails the bomb is not triggered.
  countdown--;
  if(countdown == 0)
  {
   console.log("bomb triggered");
  }
}

20. Whats the msg printed and why?
var lemein = “0”;
var lemeout = 0;
var msg = “”;
if (lemein) {
 msg += “hi”;
 }
if (lemeout) {
 msg += ‘Hello’;
}
console.log(msg);

The output is "hi" and it is because the string 0 is passed inside if statment becomes true and the number 0 is false.

21. The answer is hi and because "" is to mention that the variable will hold a string.
