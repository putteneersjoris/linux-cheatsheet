

## **foreach loops** ###


### **simple form** ###

<br>
<br>

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

💡 take notice that ``**h_text**`` is ``**not an array**``. the foreach block will loop over every element in the text. if you would want to foreach block to loop over every word. Replace ``**string h_text = "hello world";**`` by ``**string h_text[] = {"hello", "world"};**``  or by using the **split** function ``**string h_text[] = split("hello world");**`` which will reuslt in `result s@v_text:hello¶world`  
💡 **"\n"** means "make a new line"     
💡 **¶** is called the pilcrow or paragraph mark

![][vertical_text]

💡 **detail("../attribwrangle2","v_text",0)** will try to fetch a integer attribute, refernceing the first channel "0". **details(-1,"v_text")** will try to fetch a string attribute. there is no third argument.  
💡 a spare input can be added. And should be referenced as "-1" of "chs("spare_input0")" in the font sop.

<br>
<br>
<br>

### **enumerated form** ##

*enumeration:  To enumerate is to mention things one by one or to make clear the number of things. An example of enumerate is when you list all of an author's works one by one.*

<br>

The foreach with enumerated form lets you specify an **enumeration variable**:

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

<br>

<br>

```
```
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>


---











# functions #

printf(); 

%s\n =

<br>

sprintf();




[vertical_text]: https://github.com/putteneersjoris/linux-cheatsheet/blob/master/images/vertical_text.png