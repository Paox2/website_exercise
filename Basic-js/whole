4.1 Output: A table of the numbers from 5 to 15 and their squares and 
cubes, using alert. <br><br>
4.2 Output: The first 20 Fibonacci numbers, which are defined as in the 
sequence<br>
 1, 1, 2, 3, . . .<br>
 where each number in the sequence after the second is the sum of the 
two previous numbers. You must use document.write to produce 
the output.<br><br>
4.3 Input: Three numbers, using prompt to get each.<br>
 Output: The largest of the three input numbers.<br>
 Hint: Use the predefined function Math.max.<br><br>
4.4 Modify the script of Exercise 4.2 to use prompt to input a number n 
that is the number of the Fibonacci number required as output.<br><br>
4.5 Input: A text string, using prompt.<br>
 Output: Either "Valid name" or "Invalid name", depending on 
whether the input names fit the required format, which is<br>
 Last name, first name, middle initial<br>
 where neither of the names can have more than 15 characters.<br><br>
4.6 Input: A line of text, using prompt.<br>
 Output: The words of the input text, in alphabetical order.<br><br>
4.7 Modify the script of Exercise 4.6 to get a second input from the user, 
which is either "ascending" or "descending". Use this input to 
determine how to sort the input words.<br><br>
4.8 Function: no_zeros<br>
 Parameter: An array of numbers.<br>
 Result: The given array must be modified to remove all zero values.<br>
 Returns: true if the given array included zero values; false otherwise.<br><br>
4.9 Function: e_names<br>
 Parameter: An array of names, represented as strings.<br>
 Returns: The number of names in the given array that end in either 
"ie" or "y".<br><br>
4.10 Function: first_vowel<br>
 Parameter: A string.<br>
 Returns: The position in the string of the leftmost vowel.<br><br>
4.11 Function: counter<br>
 Parameter: An array of numbers.<br>
 Returns: The numbers of negative elements, zeros, and values greater 
than zero in the given array.<br>
 Note: You must use a switch statement in the function.<br><br>
4.12 Function: tst_name<br>
 Parameter: A string.<br>
 Returns: true if the given string has the form<br>
 string1, string2 letter<br>
 where both strings must be all lowercase letters except for the first 
letter and letter must be uppercase; false otherwise.<br><br>
4.13 Function: row_averages<br>
 Parameter: An array of arrays of numbers.<br>
 Returns: An array of the averages of each of the rows of the given 
matrix.<br><br>
4.14 Function: reverser<br>
 Parameter: A number.<br>
 Returns: The number with its digits in reverse order.<br><br>
 
 ``` html
 <!DOCTYPEhtml>
<html>
	<head>
		<title>The exercise</title>
	</head>
   
	<body>
	<p>exercise 4.1</p>
	<input type="button" onclick="numbers1()" value="show alert 1"/>
	<br><br><hr>
	
	<p>exercise 4.2</p>
	<input type="button" onclick="Fibonacci1()" value="show Fibonacci 1">
	<br><br><hr>
	
	<p>exercise 4.3</p>
	<input type="button" onclick="comparemax()" value="compare number">
	<br><br><hr>
	
	<p>exercise 4.4</p>
	<input type="button" onclick="Fibonacci2()" value="show Fibonacci 2">
	<br><br><hr>
	
	<p>exercise 4.5</p>
	<input type="button" onclick="validName()" value="test name">
	<br><br><hr>
	
	<p>exercise 4.6</p>
	<input type="button" onclick="sortInput1()" value="sort text 1">
	<br><br><hr>
	
	<p>exercise 4.7</p>
	<input type="button" onclick="sortInput2()" value="sort text 2">
	<br><br><hr>
	
	<p>exercise 4.8</p>
	<input type="button" onclick="no_zeros()" value="contain zero or not">
	<br><br><hr>
	
	<p>exercise 4.9</p>
	<input type="button" onclick="e_names()" value="namename">	
	<br><br><hr>
	
	<p>exercise 4.10</p>
	<input type="button" onclick="first_vowel()" value="position of leftmost vowel">
	<br><br><hr>
	
	<p>exercise 4.11</p>
	<input type="button" onclick="counter()" value="count">
	<br><br><hr>
	
	<p>exercise 4.12</p>
	<input type="button" onclick="tst_name()" value="test string">
	<br><br><hr>
	
	<p>exercise 4.13</p>
	<input type="button" onclick="row_averages()" value="each row of matrix">
	<br><br><hr>
	
	<p>exercise 4.14</p>
	<input type="button" onclick="reverser()" value="number of reverse order">
	<br><br><hr>
	</body>  
</html>
 ```
 
 ``` js
 // exercise 4.1
function numbers1(){
	var numbers = "";				// add number here
	for(var i = 5; i < 16; i++){
		numbers += i + " " + i*i + " " + i*i*i + "\n";
	}
	alert(numbers);
}

// exercise 4.2
function Fibonacci1(){
	var a = 1, b = 1;
	var numbers = "";				// add number here
	numbers += a + "," + b;
	for(var i = 1; i < 19; i++){
		var temp = a + b;
		a = b;
		b = temp;
		numbers += "," + b;
	}
	alert(numbers);
}

// exercise 4.3
function comparemax(){
	var number1 = parseInt(prompt("input the first numebr: "));
	var number2 = parseInt(prompt("input the second numebr: "));
	var number3 = parseInt(prompt("input the third numebr: "));
	number1 = Math.max(number1, number3);
	alert(Math.max(number1, number2));
}

// exercise 4.4
function Fibonacci2(){
	var n = parseInt(prompt("input a number: "));
	var a = 0, b = 1;
	var numbers = "";
	numbers += b;
	for(var i = 1; i < n; i++){
		var temp = a + b;
		a = b;
		b = temp;
		numbers += "," + b;
	}
	alert(numbers);
}

// exercise 4.5
function validName(){
	var a = prompt("input your name");
	var pos = a.search(/^[A-Z][a-z]+, ?[A-Z][a-z]+, ?[A-Z][a-z]$/);
	
	if(pos != 0){
		alert("The name you entered (" + pos + ":" + a.value + ") is not the correct form.\n" +
		"Please fix");
	}
	if(a.length() > 17){
		alert("You name too long");
	}
}

// exercise 4.6
function sortInput1(){
	var a = prompt("input: ")
	var b = a.split("");
	b.sort();
	alert(b);
}

// exercise 4.7
function sortInput2(){
	var a = prompt("input: ")
	var b = a.split("");
	b.sort();
	var c = prompt("descending(1) or ascanding(2)");
	switch (c){
		default:
			alert("input wrong");
			break;
		case "1":
			b.reverse();
		case "2":
			alert(b);
			break;
	}
}

// exercise 4.8
function no_zeros(){
	var a = [1,2,0,4,7];
	var c;
	for (c of a){
		if (c == 0){
			alert("true");
			return;
		}
	}
	alert("false");
}

// exercise 4.9
function e_names(){
	var names = ["ayy","sdfie","sdfsd"];
	var namess = new Array();
	var c;
	for (c of names){
		var a = c.split("");
		a.reverse();
		if (a[0] == 'y' || (a[0] == 'e' && a[1] == 'i'))
			namess.push(c);
		else
			continue;
	}
	alert(namess);
}

// exercise 4.10
function first_vowel(){
	var str = "sssasss";
	var st = str.split("");
	var c, a = 1;
	for (c of st){
		if (c == 'a' || c == 'e' || c == 'i' || c == 'o'|| c == 'u'){
			alert(a);
			break;
		}
		a++;
	}
}

// exercise 4.11
function counter(){
	var numbers = [1,3,0,-1];
	var neg = 0, zeros = 0, pos = 0, a;
	for(a of numbers){
		if (a < 0)
			neg++;
		else if(a == 0)
			zeros++;
		else
			pos++;
	}
	alert(neg+" "+zeros+" "+pos);
}

// exercise 4.12
function tst_name(){
	var str = "Han,Wen H";
	var pos = str.search(/^[A-Z]{1}[a-z]*,[A-Z]{1}[a-z]* [A-Z]+$/);
	if(pos != 0)
		alert("false")
}

// exercise 4.13
function row_averages(){
	var mat = [];
	var ave_row = [];
	for (a of mat){
		var c;
		for(var b = 0; b < a.length(); b++)
			c += a[b];
		c = c / a.length();
		ave_row.push(c);
	}
}

// exercise 4.14
function reverser(){
	var a = 201;
	var b = 0;
	while(a > 0){
		b = b * 10 + a % 10;
		a = a / 10 >> 0;
	}
	alert(b);
}
 ```
