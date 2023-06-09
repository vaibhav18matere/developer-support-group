### INTRODUCTION

- Programming is dynamic in nature and it cannot be managed using methods like best practices. Practice makes a good program
- Language adds structure to a program. It makes the program understandable and actionable to a developer
- JavaScript was developed by Brendan Eich in 1995 to program web pages in Netscape Navigator
- ECMAScript standard is the Universal standard for JavaScript
- ECMAScript and JavaScript can be used interchangeably—they are two names for the same language.
- Typographic conventions - the monospace font is used for code snippets

# CHAPTER 1. VALUES , TYPES AND OPERATORS

```javascript
console.log("Aardvark" < "Zoroaster")
```
<details><summary><b>Answer</b></summary>
<p>true</p>
 <p>Uppercase letters are always “less” than lowercase ones</p>
</details>


```javascript
console.log(NaN == NaN)
```
<details><summary><b>Answer</b></summary>
<p>false</p>
 NaN is supposed to denote the result of a nonsensical computation, and as such, it isn’t equal to the result of any other nonsensical computations.
</details>


```javascript
console.log(true && false)
```
<details><summary><b>Answer</b></summary>
<p>false</p>
</details>

```javascript
console.log(true && true)
```
<details><summary><b>Answer</b></summary>
<p>true</p>
</details>

```javascript
console.log(false || true)
```
<details><summary><b>Answer</b></summary>
<p>true</p>
</details>


```javascript
console.log(false || false)
```
<details><summary><b>Answer</b></summary>
<p>false</p>
</details>

```javascript
console.log(8 * null)
```
<details><summary><b>Answer</b></summary>
<p>0</p>
<p>because null becomes 0</p>
</details>

```javascript
console.log("5" - 1)
```
<details><summary><b>Answer</b></summary>
<p>4</p>
<p>"5" becomes 5 (from string to number)</p>
</details>

```javascript
console.log("5" + 1)
```
<details><summary><b>Answer</b></summary>
<p>51</p>
<p>+ tries string concatenation before numeric addition, so the 1 is converted to "1"</p>
<p>if any one is String then it just concat</p>
</details>

```javascript
console.log("five" * 2)
```
<details><summary><b>Answer</b></summary>
<p>NaN</p>
<p>When something that doesn’t map to a number in an obvious way (such as "five" or undefined) is converted to a number, you get the value NaN.</p>
</details>

```javascript
console.log(false == 0)
```
<details><summary><b>Answer</b></summary>
<p>true</p>
</details>

```javascript
console.log(null == undefined);
```
<details><summary><b>Answer</b></summary>
<p>true</p>
</details>

```javascript
console.log(null == 0);
```
<details><summary><b>Answer</b></summary>
<p>false</p>
</details>

```javascript
console.log(null || "user");
```
<details><summary><b>Answer</b></summary>
<p>user</p>
</details>

```javascript
console.log("Agnes" || "user")
```
<details><summary><b>Answer</b></summary>
<p>Agnes</p>
</details>

```javascript
var a = 100;
var b = true;
console.log(a+b);
```
<details><summary><b>Answer</b></summary>
<p>101</p>
</details>

```javascript
num = 16;
num2= null;
num+num2;
```
<details><summary><b>Answer</b></summary>
<p>16</p>
</details>

# CHAPTER 2. PROGRAM STRUCTURE

- Expressions and statements :

1. Expression ⇒ A fragment of code that produces a value ⇒ ex.  18,    "Vaibhav";

2. Statement ⇒ A full sentence ex. var name = "Vaibhav";

- Variable / ( Binding ) ⇒ Container , to keep the value (var in above example)

1. can contain digits ex. var myFav5things = "abcde" ; ✅
    
    but can't start with digits ex var 5favThings = "abcde"; ❌ 
    
2. No punctuations except dollar signs ( $ ) and  underscore ( _ ) :  
    
    ex. var me$my_javascriptNotes = "abcd";
    
3. Also don't use reserved keywords for variable name 

```
break case catch class const continue debugger default
delete do else enum export extends false finally for
function if implements import interface in instanceof let
new package private protected public return static super
switch this throw true try typeof var void while with yield
```

1. We can change variables dynamically. (It's allowed)
    
    var name = " Vaibhav";
    var name = "Matere";
    
Excercise 1 : Star pattern (one star at first linehttps://amusing-freon-21f.notion.site/Values-Types-Operators-1-05baad4e34c84398b33b5d844536458d , 2 at second and so on)
[Solution](https://replit.com/@Vaibhav18Matere/star-pattern-do-while-loop)

# CHAPTER 3 : FUNCTION
- Function declarations are not part of the regular top-to-bottom flow of control.
    - Code works, even though the function is defined *below* the code that uses it
    
    ```jsx
    console.log("The future says:", future());
    function future() {
    
         return "You'll never have flying cars";
    }
    ```
    
**Arrow function  ⇒** 

It expresses something like “this input (the parameters) produces this result (the body)”

- When there is only one parameter name, you can omit the parentheses around the parameter list.

```jsx
const square1 = (x) => { return x * x; };
const square2 = x => x * x;
```

JavaScript is extremely broad-minded about the number of arguments you pass to a function. If you pass too many, the extra ones are ignored. If you pass too few, the missing parameters get assigned the value `undefined`.

- **The call stack ⇒**
- **Optional Arguments ⇒**
- **Closure ⇒**

A function that calls itself is called *recursive*.

- **Growing functions ⇒**

**Give short and meaningful name to the function**