# 1. Setup git account in cmd

>git config user.email ***email.com***
>
>git config user.name ***your-name***
>
>// comd
>
>git config user.password ***password***




# 2. Change config globally user.name & user.email

```java
//If you want to replace the wrong ones with the proper one:

git config --global --replace-all user.name (FName LName)

//same applies for user mail:

git config --global --replace-all user.mail "mail-id@domain.com"

```
# 3. How to create a branch

```java
        <dependency>
			<groupId>org.springframework.cloud</groupId>
			<artifactId>spring-cloud-sleuth-zipkin</artifactId>
		</dependency>
```

# 3. Extensions you will need :cd:

1. **github** markdown preview by Matt Briener
2. docs-images by **Microsoft**
3. Markdown Emoji by Matt Bierner

# 4. Emoji link

You can find nice snippets on how to use emoji's and their shortcuts *here* <https://www.webfx.com/tools/emoji-cheat-sheet/>

# 5. Markdown Editors

Mac: **MacDown**
Windows: **ghostWriter** or **MarkdownEditor**

# 6. Let's Begin

Let's start by loading an Image
To load an image use the **!** exclamation symbol followed by square brackets **[]** you can pass an alternate text in the
square bracket. e.g ![Cat Image]

1. let's download the extensions we need, check the image below for reference:

![Reference image](/screenshots/picture1.jpg)
*picture 1: common markdown extensions*

2. Next create a folder anywhere and add two python files named **main.py**
and **file2.py**. i named mine **main.py** and **book**

3. Write the Code. here is the code i wrote for the **book.py**

```python
class Book():
    """This Class is an example on Python Modules"""
    def __init__(self, book_name, author, sales):
        self.book_name = book_name
        self.author = author
        self.sales = sales

    def __str__(self):
        print('Book Summary')
        return (f'Book Author: {self.author}, Book Name: {self.book_name}, Sales: {self.sales}')

    def AboutBook(self):
        print('An enchanting story about a young kid called Alex')

``` 
4. Next Here is the code i wrote for the **main.py** file

```python
# importing the book module 
#import pygame
import book

#pygame.init()
# creating instances of the book 
ebook1 = book.Book('Arabian Nights', 'Muhammed Ali', 1000000)
print(ebook1)

# accessing the methods of the class 
ebook1.AboutBook()

```
Running the program we get the following output shown in the image below 

![image showing program output](/screenshots/picture2.jpg)
*Image 2: results of running the main program*

# Summary

That's how you can create a nice README file for markdown. You can find this 
script file on the *githublink* <https://github.com/mahmus-fifi/python_modules_lesson.git> below or reach me via mail <101touchapps@gmail.com> 
-
