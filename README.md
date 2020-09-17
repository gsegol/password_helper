
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

Password managers are commonly used to generate and store complex and unique passwords.  However, a user may find it convenient to memorize the passwords of a few accounts so that they can be accessed even if the password manager is unavailable. This project is intended to generate a password that is sufficiently complex to be secure, yet provides enough clues to the account owner to remember it easitly.

The basis of this technique is a use of a 'phonetic alphabet" whereby the letters of the alphabets are converted into one of the 0-9 integers (see Ref 1).
The program works as follows:
1. start with a phrase provided by the user (e.g., 'my name is Bond, James Bond'
2. remove space, punctuation, and vowels from the phrase
3. select randomly a number of letters to be converted according to the phonetic alphabet
4. return the alphanumeric password corresponding to the initial phrase

a password for the sample phrase above could be:
'3nms92djm0bn1'
or
'mnm0b2d6m0921'
Note:  Feel free to change some lower-case letters to capital leters and add special characters if desired.

Phonetic alphabet
         letter
1          d, t
2             n
3             m
4             r
5             l
6     j, sh, ch
7          k, g
8          f, v
9          b, p
0   s, x, z, th

vowels, h, and w are ignored


## File Descriptions <a name="files"></a>

There are a single .py classes in addition to the standard setup and license files.

## Results<a name="results"></a>

USAGE:
You can import the Pwd_helper class and use it from the command line.
e.g. 
>>from password_helper import Pwd_helper()
>>helper = Pwd_helper('your phrase')
>>helper.make_alphanum()

the alphanumeric password is returned as a string

#to print the phonetic alphabet:
>>helper.phonetic

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
The license files define the standard legal verbiage. Otherwise, the code is free to use.
