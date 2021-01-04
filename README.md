![ramon-salinero-vEE00Hx5d0Q-unsplash.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1609770440471/FSQ8fo9bL.jpeg)
Data is the most important component in the computer used to define information and stored as sequence of bits.
**Bits** define as zero's and one's.
#### How to express a number in bits?

Lets take a number 15,

| 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |
| --- | --- | : --- | : --- | :--- | :--- | :--- |
|128 |64 |32 |16 |8 |4 |2 |1 |

So, 00001111 is the binary number for 15. Its non zero digits stands  for 8,4,2 and 1 and after adding them result came as 15.

## Values
***
Modern computer has more than 30 billion bits in its working memory. Challenging task is to work with that much amount of bits without making mistakes, so we need to make chunks of information. Those chunks are called as **values**. Now the point is that all values are made of bits of different size. Value has a different type as text or numbers or functions. 

#### How do we create value?

To create value you just need to invoke its name and need to store some where.

### Numbers

Number is define as numeric values. In JavaScript it is written as,

20

JavaScript uses 64 fixed numbers of bits to store a single number.

**1. Arithmetic**


Arithmetic operation can be done with the numbers. Arithmetic operation like addition, multiplication, division or subtraction take two numbers and produce a new number.

#### How to add two numbers?
100+4 = 104

The '+' symbol is called as **operators**, need for addition operation.
There is list of arithmetic operators such as,

| Operator | Description |
| ------ | -------------- |
|  +  | Addition |
| -  | Subtraction |
| * | Multiplication |
| / | Division |
| % | Modulus |
| ** | Exponential |
| ++ | Increment |
| -- | Decrement |

**2. Special Numbers**

There are three types of special number in JavaScript considered as number but not behave like numbers. The first two is -infinity and + infinity which represents the negative and positive infinities and next special number is NaN. 
**NaN** is stands for not a number and you will get this as result when you try to calculate like 0/0 or infinity-infinity or other operation that end up of giving meaningless result.

## Strings
***
Strings are considered as basic data type in JavaScript  and used to represent text by writing the content within quotes. Such as,

"Hello my friend"

Three ways to write strings are using,
- using single quotes(' ').
- using double quotes(" ").
- using backticks(`).

Strings need to be handle in series of bits. JavaScript use **Unicode** standard to assign number to every character that you need. So the strings can be written by series of numbers.

#### '+' Operator in String

Arithmetic operation with string is not possible but  '+' operator can be use by string to concatenates. Concatenation is a way to write different strings together. Such as,
"con"+"cat"+"e"+"nate"

#### Template Literals

Backtick quoted strings are called **template literals**. If you want to embed values within the string you can achieve by using backtick. Such as,
```
`multiplication of 2 with 2 is ${2*2}.`
 -> multiplication of 2 with 2 is 4.
``` 
When you just write something within **${ }**, its result will be calculated and converted to string in that position.

### Unary Operators
***
Operators that takes one values are called **unary operators**.
As example,
```
console.log(-(10-2))
//-> -8
```
> NOTE:- minus operator can be used as bitwise operator and unary operator.

There is  **typeof** operator present which is not a symbol. It produces string value defines the type of value you give it.
```
console.log(typeof 5)
//-> number
```
#### Boolean Values

Boolean type has just two values true and false. It is useful when you have to choose between two possibilities like 'yes' or 'no'.

**Comparison**
 is the way you can produce boolean values.
```
console.log(8>12)
//-> false
```
The > and < signs are the greater than and less than symbol comes under binary operators.

Above one was for numbers but,

** How to compare two strings?**

In a same way strings also be compared.
```
console.log("Oman" < "Surat")
//-> true
``` 
>NOTE:- uppercase letters are always less than lowercase ones so "S" < "s".

### Logical Operators
***
Logical operators use to do some operation with boolean values themselves. There are three types of logical operators as,
- And
- Or
- Not

The && operator is a logical *and* comes under binary operator. Gives value as true if both the values given to it are true.
```
console.log(true && false)
//-> false
console.log(true && true)
//-> true
```
The | | operator is a logical *or* comes under binary operator. Gives true if one of the values given to it is true.
```
console.log(true || false)
//-> true
console.log(true || true)
//-> true
```
The !(Not) operator  is under unary operator unary operator  and flips the value given to it.

`!true=false`
### Empty Values

There are two special values **null** and **undefined**.

**Null**
- null is an empty value and must be assigned.
```
let b= null;
console.log(b);
//-> null
```

**Undefined**
- Undefined means when a variable has been declared and not assigned with value or defined.
```
let b;
console.log(b);
//-> undefined
```
>NOTE:- (null !== undefined) its true because null does not strictly equal to undefined but (null==undefined) is true because they are loosely equal.

### Automatic Type Conversion
JavaScript can accept almost any programs that you give it even with odd things also.
```
console.log(8 * null)
//-> 0
console.log("5" - 1)
//-> 4
console.log("5" + 1)
//-> 51
console.log("five" * 2)
//-> Nan
```
When JavaScript get to know about that the operator applied to the wrong value, it just convert that value to the type it needs. This is called type correction.

When something is not mapped to a number particularly it just convert it to a number with value Nan. Any further arithmetic operation with Nan produces Nan only.

### Short Circuiting of Logical Operator
***
Short circuiting is a way of avoiding unnecessary workload. In JavaScript logical operator contained expression is evaluated from left to right until it is confirmed with that the result of the other condition is not going to effect the previous result. If the result is clear before complete evaluation of the expression, it just short circuit and give result.

**AND**

For the case of *and* operation, expression will be evaluated until you get one false, that makes result as false without depending further condition.
```
console.log(false && true)
//-> false
```
**OR**

For the case of *or* operation, expression will be evaluated until you get one true, that makes result as true without depending further condition.
```
console.log(false || true)
//-> true
```

### Summary
***
We covered four types of values numbers, strings, booleans and undefined values.

