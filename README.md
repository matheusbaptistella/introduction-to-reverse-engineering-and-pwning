# Introduction to Reverse Engineering and Pwning
This repo aims to be a material on information about cybersecurity, specifically, **reverse engineering**. Not only it will present to the reader the concepts related to vulnerabilities and their exploits, but also contain **practical examples** to make the learning process more dynamic. This material is being written by myself: currently I'm a  student at Universidade de São Paulo (USP), under a Computer Engineering degree. The objective is to write down all the knowledge taht I've acquired on reverse engineering during graduation, in the most **comprehensive** way, so I can keep visual track about what I've learned and anyone that feels interested about this subject may read and learn it, just as I did. 

Although it's impossible to truly understand the conditions which makes programs vulnerable without getting deeper into processor and memory concepts, my goal is to make the explanation seems **as natural as possible**. Essentially, I'll start from initial exploitation techniques, such as Buffer Overflow and Shellcode, but as I gradually advance my studies and gather more knowledge, I'll **update** this material with new information.

## Structure
For each vulnerability covered in this repo, there will be a corresponding directory with the name of that vulnerability, for example: the complete material, with explanation and examples, about Buffer Overflow will be in the directory with its name on it. Inside each directory, there will be a theory-introduction file, which will contain the theoretical explanation about that directory's vulnerability, and another directory with the practical examples. In addition, I'll classify each directory with an order to study, divided in parts. So under `part1-buffer-overflow` directory (note that it's part 1, so it should be the first subject studied), `README.md` file contains the explanation about the Buffer Overflow subject and `examples` directory, the pre-made examples.

## General Requirements
* C programmig language;
  * Reverse engineering has an intrinsic relation with memory, so, in order to explain it and create examples that manage memory usage, we'll use C.
* x86_64;
  * This will be the architecture used for explanation in general, and it's easier to comprehend if you already know about this architecture's instructions and registers.
* Linux terminal;
  * Basic commands, VIM and GDB.
* Python3.
  * Initially, python will be presented with the use of `pwn` library.

Whereas this knowledge is required, **do not panic** if you're not sure how much you know about it all: if a vulnerability needs some technichal concepts to be widely-comprehended, I'll explain it, but, for now, this material tends to be less detailed than an entire graduation course, therefore it's important to be familiar with these requirements.

## So, what's reverse engineering?
In a more general meaning, to reverse engineer an object is to analyze its properties, the way it was contructed and the very components that, altogether, make it behaves properly, in order to **fully understand** the functioning of that particular object. When referring to computer science, to reverse engineer a progra, is to make use of techniques and tools to gather information about its source code, that is, to map how its methods works, how it treats input data and so on, with the final purpose of  being able to **manipulate** it purposely. Cybersecurity professionals will attempt to reverse engineer the code they're responsible for, in order to find out if it's vulnerable to any sorts of attacks.
