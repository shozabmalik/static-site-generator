# Utils/html_checker.py
Useful Resources: 

- HTML.Parser python doc(https://docs.python.org/3/library/html.parser.html)

- Understanding Super (https://realpython.com/python-super/)

- Argeparse - (https://docs.python.org/3/library/argparse.html)

-

Understanding Sections of code:


**from html.parser import HTMLparser**

This module defines a class HTMLParser which serves as the basis for parsing text files formatted in HTML

An HTMLParser instance is fed HTML data and calls handler methods when start tags, end tags, text, comments, and other markup elements are encountered. The user should subclass HTMLParser and override its methods to implement the desired behavior


**from html_content_spec import content_spec, _ANY_CONTENT, _NO_CONTENT**

This import receives the content_spec hash map from html_content_spec.py with keys representing HTML tags


**import argparse**

This module essentially reads command-line arguments and feeds them to the program. It is a command-line parsing module

**Class OurHTMLParser**    

Class OurHTMLParser is the descendant of HTMLParser and only overrides necessary methods

    def __init__(self):  # type: () -> None

        super(OurHTMLParser, self).__init__(convert_charrefs=False)


super() gives you access to methods in a superclass from the subclass that inherits from it. super() alone returns a temporary object of the superclass that then allows you to call that superclass's methods.

super() can also take two parameters: the first is the subclass, and the second parameter is an object that is an instance of that subclass.

super() works in single and multiple inheritance.

# Utils/create_menu.py

Creates a menu from a tab-delimited text file







