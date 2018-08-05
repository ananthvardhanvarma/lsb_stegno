# lsb_stegno
Stegnography Program written in python which hides the desired text into
the image file (*.png).
Image format supported to hide text is **PNG**

## Algorithm
The encryption relies on hiding the hiding the test in last bits of hex codes:

> Suppose your plainText is b'01'
> and your 7 digit hex code is something like **7654321** here digits representing respective positions. 
so the algorithm will start replacing the *least significat bits* from the rgb values with the text values 
so in this case 765432_ here 1 will be replaced by '0' resulting 7654320 and when all the text values will 
be replaced then **1111111111111110** will be appended in the end of the string so when decrypting we know
when we reached the end.

## Dependecy
Using PIL library for retrieving the hex values

## Usage
Place the PNG image file in the root folder  and run using hide.py


