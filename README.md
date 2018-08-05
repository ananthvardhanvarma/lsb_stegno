# lsb_stegno
Stegnography Program written in python which hides the desired text into
the image file (*.png).
Image format supported to hide text is **PNG**

## Algorithm
The encryption relies on hiding the hiding the test in last bits of hex codes:

> Suppose your plainText is b'11'
> and your 7 digit hex code is something like **7654321** here digits representing respective positions. 
