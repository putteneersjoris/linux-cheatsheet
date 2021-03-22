# this is a header
## this is a header
### this is a header
#### this is a header
##### this is a header
###### try this

you can add lines using "tab"     
and it actually works   
like this


this one is **bold**    
this one is *italic*    
this one is ***bold italic***   

### this is how you add **line breaks**
<br>
<br>
<br>

> this is how you write a "blockquote"   
>> nesting 
>>> nesting

<br>
<br>
<br>

### **non-ordered lists**

>### embed other elements   
> - like this
> - or this    
>     - or like this  
>     - or so
> - or maybe this  
>    
> looks *pretty* **good**

### **ordered lists**
1. test
2. test
3. test
   1. test
      1. another test
      2. and another
   2. test
4. test  


<br>

## this is how to add a **seperator**
<br>

___

<br>

## this is how to add **links**

<br>

**inline style link**

I really like this [guy](https://jorisputteneers.tumblr.com/)

<br>

**inline style link with title**

I really like this [guy](https://jorisputteneers.tumblr.com/ "this really is a cool guy you know")


<br>

## this is how to add **images**

1. from websites

    in text ![](https://64.media.tumblr.com/e91f2aebada91eb434526d4e3a69aecd/629e195c885c6ee5-78/s1280x1920/dbab335118b622ddd49c1695b97428a5036df9ab.jpg)



    or with a variable
    ![][me with jobot]



    [me with jobot]: https://64.media.tumblr.com/e91f2aebada91eb434526d4e3a69aecd/629e195c885c6ee5-78/s1280x1920/dbab335118b622ddd49c1695b97428a5036df9ab.jpg

2. from the github rep

    ![tux](https://raw.githubusercontent.com/putteneersjoris/linux-cheatsheet/master/tux.png)

## this is how to imbed **youtube videos**

![rickrolled](https://www.youtube.com/watch?v=dQw4w9WgXcQ)

### this is how to add **code blocks**

inline `code` has \`backtips` to it 

these pieces of code will count the even numbers between a starting value and an end value. 

<br>

#### **Python syntax**

```python
def count_even_numbers(begin, end):
    counter = 0
    for i in range (begin, end):
        if i%2 ==0:
            counter +=1    
    print("there are: ",counter, "even numbers between :",begin, " and ",end,)
def main()
    count_even_numbers(0,50)
main()

```
Python code output result: 
```
there are 25 even numbers between 0 and 50
```

#### **C syntax**
```C++
function void count_even_numbers(int begin; int end;){
    
    int count = 0;
    for(int i = begin ; i < end; i++ ){   
        if(i%2){count += 1;}       
      }
    printf("%s\n","there are "+itoa(count)+" even numbers between "+itoa(begin)+" and " + itoa(end));
   }
   
function void main(){count_even_numbers(1,50);}
    
main();

```
VEX code output result:

```
there are 25 even numbers between 0 and 50
```

## this is how to add **color** 

( we'll have to use html, and a parser who supports html. git for example, does not support html)

<span style="color:red">some **red** text</span>

or we'll use emoji's as colored marks

🔴🟠🟡🟢🔵🟣🟤⚫💡
