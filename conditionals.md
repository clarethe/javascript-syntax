<h1 align="center">
<br>
<br>
<img src="./images/making-decision.png" />
<br>
Making decisions in your code — conditionals
<br>
<br>
<img src="./images/js-operators.jpeg" />
<br>
</h1>
 

[![Visitor](https://visitor-badge.laobi.icu/badge?page_id=clarethe)](https://github.com/clarethe) [![GitHub followers](https://img.shields.io/github/followers/clarethe.svg?style=social&label=Follow)](https://github.com/clarethe?tab=followers)

In any programming language, the code needs to make decisions and carry out actions accordingly depending on different inputs. For example, in a game, if the player's number of lives is 0, then it's game over. In a weather app, if it is being looked at in the morning, show a sunrise graphic; show stars and a moon if it is nighttime.

## if...else 

```
if (condition) {
   statement1
} else {
   statement2
}
```

**`condition`** 
Typically "is this value bigger than this other value?", or "does this value exist?". The condition makes use of the comparison operators we discussed in the last module and returns ```true``` or ```false```.

**`statement1`** 
Statement that is executed if condition is ```truthy```.
<br>

**`statement2`** 
Statement that is executed if condition is ```falsy``` . 

Multiple if...else statements can be nested to create an else if clause. Note that there is no elseif (in one word) keyword in JavaScript.

```
if (condition1)
  statement1
else if (condition2)
  statement2
else if (condition3)
  statement3
...
else
  statementN
```

## Switch

If...else statements are mainly good for cases where you've got a couple of choices or the conditions are complex (for example, multiple logical operators). 

 **`Switch statements`** are your friend for cases where you just want to set a variable to a certain choice of value and find one that matches executing the corresponding code that goes along with it. 

 ```
 switch (expression) {
  case value1:
    //Statements executed when the
    //result of expression matches value1
    [break;]
  case value2:
    //Statements executed when the
    //result of expression matches value2
    [break;]
  ...
  case valueN:
    //Statements executed when the
    //result of expression matches valueN
    [break;]
  [default:
    //Statements executed when none of
    //the values match the value of the expression
    [break;]]
}
 ```

**`expression`**
An expression whose result is matched against each case clause

**`case (Optional)`**
A case clause used to match against expression.

**`default (Optional)`**
A default clause; if provided, this clause is executed if the value of expression doesn't match any of the case clauses.


## Ternary operator
This can be useful in some situations, and can take up a lot less code than an if...else block if you have two choices that are chosen between via a true/false condition. 

 ```
 condition ? exprIfTrue : exprIfFalse
 ```

**`condition`**
An expression whose ```value``` is used as a condition

**`exprIfTrue`**
An expression which is evaluated if the condition evaluates to a ```truthy```

**`exprIfFalse`**
An expression which is executed if the condition is ```falsy``` 

Example:

```
var age = 26;
var beverage = (age >= 21) ? "Beer" : "Juice";
console.log(beverage); // "Beer"
```


Possible falsy expressions are: ```null```, ```NaN```, ```0```, empty string ```("")```, and ```undefined```. If condition is any of these, the result will be the expression ```exprIfFalse```.

