
# Loops and flow control

# **1. Foreach loops** 

<br>
<br>

## **Simple form**

This loops over the members of **array** . For each iteration, it **copies** the current member to value " i" and then executes the given statement.

**example1: print integer array**
```` C
int array[] = {1,2,3,4,5,6};
foreach(int i; array){
    printf("%d", i);
    }
````
`result "printf": 123456`

<br>
<br>

**example 2: print float array**

```C
float float_array[] = {0.0,1.0,2.0,3.0,4.0,5.0,6.0};
foreach(float i; float_array){
        printf("%f",i);
        }
```
`result "printf": 0.0,1.0,2.0,3.0,4.0,5.0,6.0`

<br>
<br>

**example 3: print string array**

```C++
string string_array[] = {"A","B","C","D","E"};
foreach(string i; string_array){
    printf("%s", i);
    }
```
`result "printf": ABCDE`  

<br>
<br>

**example 4: make horizontal text, vertical using a foreachloop (simple form).**

```C
string h_text = "hello world";
string newtext;
foreach(string i; h_text){
    append(newtext,i+"\n");
}
s@v_text = newtext;
```
`result s@v_text: h¶e¶l¶l¶o¶ ¶w¶o¶r¶l¶d¶` 

💡 take notice that **h_text** is **not an array**. the foreach loop will loop over every element in the text. if you want the foreach loop to loop over every word. Replace ``string h_text = "hello world";`` by ``string h_text[] = {"hello", "world"};``  or by using the **split** function ``string h_text[] = split("hello world");`` which will result in `s@v_text:hello¶world`  
💡 **"\n"** means "make a new line"     
💡 **¶** is called the pilcrow or paragraph mark

![][vertical_text]

💡 **detail("../attribwrangle2","v_text",0)** will try to fetch a integer attribute, referencing the first channel 0. **details("../attribwrangle2","v_text")** will try to fetch a string attribute. there is no third argument.  Notice the "s" on details.
💡 A spare input can be added. And should be referenced as "-1" or "chs("spare_input0")" in the SOP.

<br>
<br>
<br>

## **Enumerated form**

*enumeration:  To enumerate is to mention things one by one or to make clear the number of things. An example of enumerate is when you list all of an author's works one by one.*

<br>

The foreach loop with enumerated form lets you specify an **enumeration variable**:

For each iteration, **this form assigns the current position in the array to index**, copies the current member to value, and executes statement. For example:

<br>
<br>

**example 1: add the "place" of the current element to that element and print it out**

```C
string text = "Hello Wold";
string newtext;
foreach(int j; string i; text){
    append(newtext, i + itoa(j)); 
}
printf("%s",newtext);
```
`result: H0e1l2l3o4 5W6o7l8d9 `

💡 the **"itoa"** function returns a string value from an integer.

<br>
<br>

**example 2: print which day of the week it is in the format: "Mo is day 1 of the week (using the enumerated form)**
```C
string days_of_the_week[] = {"Mo","Thu","Wed","Thur","Fri","Sat","Sun"};
foreach(int k; string i; days_of_the_week){
    printf(" %s is day %d of the week ",i,k+1);  
    }
```
`result:  Mo is day 1 of the week  Thu is day 2 of the week  Wed is day 3 of the week  Thur is day 4 of the week  Fri is day 5 of the week  Sat is day 6 of the week  Sun is day 7 of the week `


visualization of one cycle: "Mo" is the first element of "days_of_the_week". "Mo"is copied to value **i**. The numerator **k** diplays the position in the array which is 0.

![][//numerator]

<br>
<br>
<br>

# **2. For loops**

<br>
<br>
   
i++ vs ++i

TO BE CONTINUED

what is foo? 

---

# functions

## **printf() & sprintf()**
`void printf(format, ... )` `string sprintf(format, ... )`

<br>
<br>

whilest ``printf()`` returns a void, ``sprintf()`` returns the result as a string instead of printing it.

When a % symbol is found in the format string, an argument will be printed out in the format specified by the characters following the % symbol. 


- %f print a float
- %d print a integer 
- %e print a float vector
- %p print an integer vector
- %s print a string
- %x print a variable in hexidecimal

examples: 

💡 %s\n =

TO BE CONTINUED




















[numerator]: https://github.com/putteneersjoris/linux-cheatsheet/blob/master/images/numerator.jpg
[vertical_text]: https://github.com/putteneersjoris/linux-cheatsheet/blob/master/images/vertical_text.png