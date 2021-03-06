# General Formatting

## Headings
```
# This is a H1 header
```
# This is a H1 header
```
## This is a H2 header
```
## This is a H2 header
```
### This is a H3 header
```
### This is a H3 header

## Bullet Points:

### Use "* " to create a bullet point (note the space after)
```
* This is a bullet point!
```
* This is a bullet point!

### Use " * " to create a secondary point (note the space before)
```
* Primary bullet!
  * This is a secondary bullet point!
```
* Primary bullet!
  * This is a secondary bullet point!

## Text Manipulation

### Bold
```
**This text is bold**
```
**This text is bold**

### Italic
```
*This text is italic*
```
*This text is italic*

## Links

### External link
```
[This is google](http://www.google.com)
```
[This is google](http://www.google.com)

### Internal Link (actual)
```
[ [electrode] ] 
```
*without the spaces in between, won't display here if left out
[[electrode]]

### Internal Link (different)
```
[electrodes](electrode)
```
[electrodes](electrode)

## Pictures
```
![Alt text](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)
```
![Alt text](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)

## Escape Characters
If you need to use links with parentheses or want to use characters in text that are used for Markdown formatting (eg: *, [, ], #, etc) use a backslash "\" followed by the character to use it in text
```
# this is a header
\# this is not
```
# this is a header
\# this is not

## Code
Type \``` three times before and after code (note this is not an apostrophe, same key as ~)
You can also use a specific language by specifying it \```python
```python
for i in 1:10
```

## Footnotes
```
Something special<sup id="a1">[1](#f1)</sup>
```
Something special<sup id="a1">[1](#f1)</sup>
```
<b id="f1">1</b> Footnote content here. [↩](#a1)
```
<b id="f1">1</b> Footnote content here. [↩](#a1)

Note, this is a manual footnote, it will not update according to its order on the page.