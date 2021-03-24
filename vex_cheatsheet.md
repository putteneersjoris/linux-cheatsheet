

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


💡 **"\n"** means "make a new line"     
💡 **¶** is called the pilcrow or paragraph mark

![][vertical_text]

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

```
ss

```
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