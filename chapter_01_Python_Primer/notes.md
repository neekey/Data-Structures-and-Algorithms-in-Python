# Notes

## Use `raw_input()` instead of `input()`

[Python unexpected EOF while parsing from input()](http://stackoverflow.com/questions/5074225/python-unexpected-eof-while-parsing):

> If you use `input`, then the data you type is is interpreted as a Python Expression which means that you end up with gawd knows what type of object in your target variable, and a heck of a wide range of exceptions that can be generated. So you should NOT use input unless you're putting something in for temporary testing, to be used only by someone who knows a bit about Python expressions.
> raw_input always returns a string because, heck, that's what you always type in ... but then you can easily convert it to the specific type you want, and catch the specific exceptions that may occur. Hopefully with that explanation, it's a no-brainer to know which you should use.
