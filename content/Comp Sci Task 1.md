---
layout: default
---
# Comp Sci Task 1

1. State the problem
**Description**
- The core idea of the program is a voice assistant targeted for high-school students as a useful tool in managing and optimising their work/study life on the computer.
- I've titled the program **Ed's Voice Assistant**, as it is a voice assistant made by me.
- The program is a personal tool app. It is not designed to be used for educational purposes, and while it caters for improving the education quality of high-school students, it does not directly provide education. It may also be considered an entertainment app, but its primary focus is as a digital tool to improve a user's interaction with their computer.
- Once initialized, the voice assistant will listen to the user and execute a range of functions, such as opening Firefox, opening Obsidian (note-taking app), etc. There is also some quality-of-life functions for the program, such as closing the program.
- As stated before, the target audience is students, as I feel that most students could use a voice assistant in terms of managing and further optimizing their computer usage, aiming predominantly for greater ease of use. 
- I aim to create a voice assistant that will allow increased productivity when using their computer for study or work. The target audience, myself included, wish to increase their personal productivity when studying, by eliminating repetition and tediousness that occurs regularly. 
	- For example, when I am studying chemistry, I open Firefox, Obsidian and OneNote, and open textbooks I have on my computer. This takes valuable time, and reduces my overall efficiency when studying. I plan for my voice assistant to remove this inefficiency, by allowing custom commands, where if I were to say a key phrase, it would do all of these things at once, saving me crucial time.
	- In the future, I also plan for the voice assistant to be a general tool in the office, for example it could send emails to large batches of fellow colleagues. 
	- Furthermore, people who have used voice assistants before may demand high quality in graphical design of the program. Using Tkinter, I plan to provide a well-thought-out visual interface, however **I have used copyrighted images (Siri logo) for parts of the visual design**, as I feel its simplistic design fits my program, and I admire the quality of the Siri voice asssitant.
- The program will fill its user's need for a simplistic, easy-to-use voice assistant that will improve their productivity. It will also improve their quality of life, by helping its users achieve a healthy study schedule/routine.
- The licencing used is the Permissive MIT licence, the reasoning for which is explained at the end of the Licencing section.

**Licencing**
Currently, there are 3 main software licences used by companies across the world:
- *Permissive*
	- **Examples:**
		- BSD licences (family)
		- MIT Licence
		- Apache Licence
		- ISC Licence
		- JSON Licence
	- Permissive licences are a kind of free-software licence, which means it is allows users to run the program the licence is attached to, analyse the code of the program, and most importantly redistribute modified version of the program under whatever licence fits. This essentially allows developers to configure a program how they see fit, and release their new program under a new licence.
	- Permissive licences are also very compatible with other licences, due to its minimal restrictions on the user.
	- *It should be noted that a crucial flaw with Permissive licences is that they do not guarantee the type of licence of derivative software, and thus can result in derivative programs that are not free or publicly available.*
	- There are a few requirements for users of a program under a permissive licence, if they wish to redistribute the software:
		- They must leave in the original copyright notice.
		- They must leave the initial licence text of the program, such as the one shown below:
```yaml {title="MIT License text"}

_Begin license text._

---

Copyright <YEAR> <COPYRIGHT HOLDER>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

_End license text._

```
- *Copyleft*
	- **Examples:**
		- GNU General Public Licence
		- GNU Lesser General Public Licence
		- Mozilla Public Licence
		- Open Software Licence
		- Microsoft Reciprocal Licence
	- Copyleft licences are considered generally quite restrictive, and require that the same established rights in the license of the initial software remain in any derivate programs. However, Copyleft licences are still considered relatively open-source, as like Permissive licences, they grant many user freedoms, such as:
		- Right to perform/display, i.e. the right to use/display the program in public
		- Right to modify
		- Right to distribute
	- However, compared to Permissive licences, Copyleft licences do not allow users intending to redistribute modified software to include sublicences. In general, Copyleft licences also stipulate that redistributed version of software must keep the source code available to recipients of the new software. Furthermore, any derivative version must have the same licence as the initial software.
	- **The core difference between Copyleft and Permissive licences is that Copyleft licences require that any derivate programs contain the same licence.**
- *Commercial/Proprietary*
	- **Examples**
		- There are no examples of public licence for Proprietary and Commercial software, as in general companies create specific legal agreements between them and users.
	- Proprietary/Commercial licences are some of the most restrictive licences available for software.  Minimal amounts of users are usually given, such as rights to use and display the program. However, the use of software under Proprietary or Commercial licences are usually highly restrictive.
		- For example, Adobe licences used to be limited to one users, i.e. they could only be used on one computer at a time.
	- Commercial and Proprietary licences are generally considered *closed-source*, as most Proprietary and Commercial programs are distributed in their **compiled form**, compared to **source code**.
	- In general, Commercial and Proprietary licences also heavily restrict the redistribution of software. Where source code is available, some Proprietary and Commercial licences also restrict the distribution of modified source code.

Having research many software licences, I have settled on using the MIT licence for my program. I believe this licence reflects my desires for the use of my program, as I hope that others can take the program and improve on it for their own use. I also believe that if their version of my voice assistant is both unique and helpful for others, that its developers should be able to relicense it.

**Resources**
The program is Python based, and relies on text files to store data. The program also requires a lot of modules for its basic function:

*Modules:*
| Module Name        | Purpose                       | Importance          |
| ------------------ | ----------------------------- | ------------------- |
| tkinter            | GUI Design                    | Essential           |
| pyttsx3            | Outputting voice              | Essential           |
| speech_recognition | Recognising user input        | Essential           |
| PIL                | Getting images                | Moderate Importance |
| atexit             | Running code when script ends | Moderate Importance |
| fileinput          | Closing text files            | Low Importance      |
| sys                | Debugging in console          | Low Importance      |
| time               | Getting time for the user log | Low Importance                    |

There is minimal equipment requirements for the creation and development of this program. I used a relatively high-end Dell XPS-15 and Visual Studio Code for the development of the software. However, I had to install Python 3.10, and also all the modules listed above through PIP installation.

For Visual Studio Code, I had the *Pylance* and *Python* modules installed. *Pylance* offers **rich type information**, i.e. gave suggestions for minor things for code, e.g. parameters, while the *Python* module allowed me to run and write the code in Visual Studio Code.

I also used multiple sources of documentation for the various libraries for the program, such as Python Tutorial's website(https://www.pythontutorial.net/tkinter/), Tkinter documentation in Python(https://docs.python.org/3/library/tk.html), the official documentation of pyttsx3(https://pyttsx3.readthedocs.io/en/latest/), etc.

In terms of skills and expertise, I have moderate skills in Python coding. I have a strong understanding of how functions work, which prove incredibly important for managing the structure of the program (having a main function, having a function that takes user voice input, having a function that speaks, etc.). Furthermore, through a strong understanding of lists, dictionaries and the use of text files in Python, I was able to store user data in a text file, and log all user interactions with the program in another file.

I decided to log the actions of the program, as I felt that this would prove quite helpful as a means of gauging errors in the. However, I did not get to be able to log the change in variables present throughout the program, which means the logs will most likely be unhelpful for fixing logic errors.

Visual Studio Code was my main source of testing for the program. Through its debugging menu (F5), I initially worked on the raw main.py file. I did so because when I pressed the Run Python File button, it did not access the text files. Later on while working on the project, I realised that I needed to open the folder the program was in, and from then I started using the Run Python File button, as it was easier to use.

I also used Stack Overflow as a source of advice in using complex/badly-designed modules, such as Tkinter. For example, I initially had a problem with creating a function which would create multiple buttons of the same function, but with different parameters. I had difficulty fixing this issue, as I found that when the program started up, all the buttons were essentially pressed once, and would be unusable after. 

```yaml {title='Button Code'}
for i in accountdata:

        button = ttk.Button(text = str(i))

        button['command'] = finduser(i)

        button.pack()
```
/* Note that the "finduser" function is a separate function.

However, after looking up this issue with Tkinter on Stack Overflow, I discovered that when Tkinter parses through the 'command' section, it interprets the brackets as calling the function, and immediately calls the function, while incorrectly parsing the function, making it un-callable by the user.

I also learnt from Stack Overflow to instead use Python's lambda functions.

```yaml {title='Improved Button Code'}
for i in accountdata:

        button = ttk.Button(text = str(i))

        button['command'] = lambda i=i: finduser(i)

        button.pack()
```

**Similar Products**
- *Alexa*
	- Amazon's Alexa excels in its compatibility with many operating systems, such iOS and Android. It also has numerous unique commands, and even includes voice commands that can change settings. I have considered using voice-activated commands to change settings, but I feel there is simply not enough settings to change, and it would be redundant. Furthermore, as the program is a python file, it is generally incompatible with most computers, considering the amount of modules it relies on.
- *Google Assistant*
	- Google Assistant's greatest quality is its voice recognition software, which is some of the best in the world. However, through Google's text-to-speech module in Python, my voice assistant should have the same recognition capabilities. Stylistically, Google Assistant has a simplistic, colourful design, which I have been inspired by. The design of Google's voice assistant focuses on user interaction, in its friendly voice and extensive utility as a general assistant. I am able to use Google's text-to-speech via its Python module
- *Siri*
	- Apple's Siri is a very versatile voice assistant. It has limited settings, and is not very compatible compared to other well-known voice assistants. However, in terms of languages available, Siri is quite compatible, supporting up to 21 languages as of April 2021. Siri is mostly designed for mobile uses, which is why it is the most popular voice assistant for mobile devices. Unfortunately, as my program is written primarily in Python, and requires a lot of Python modules, it is incompatible for mobile use. However, I hope to design a voice assistant with much more basic voice commands than Siri, and my idea of customised voice commands give my program an advantage over Siri.
2. Plan and Design
**Screen Layout**
Initial Layout:
![](000_Files/Pasted%20image%2020220912213050.png)
- I've intentionally moved it off to the corner. I feel that voice assistants should be subtle in their location, and having it stuck in the middle would be confusing and weird for the user to use. 
- I personally worked on the design for the favicon logo and the central logo for the program.
	- The design features the logo of Siri, with inverted colours, surrounded by 1 thick circle and 2 thinner circles, under a chromatic background, with a plus symbol in the bottom right corner.
		- The reasoning for the Siri logo is because Siri is a popular voice assistant, one which I am inspired by in its accessibility and ease of use.
		- I feel the chromatic background will appeal to younger audiences, as it gives a sense of modernity. In doing so, I've attempted to entice young high-school students into using my program.
		- The plus sign is found in other projects of mine, as an inside joke.
		- The circles surrounding the Siri logo add a sense of modernity and class to the logo.

Turning on the Program:
![](000_Files/Pasted%20image%2020220912213713.png)
![](000_Files/Pasted%20image%2020220912213732.png)
- Here I've decided to use 2 windows, as otherwise I would have run into issues with removing the central logo image of the initial window.
- I've included a little bit of code that **scales the height of the second window, relative to the number of accounts stored in the program**, so that the window can accommodate for as many account as can fit on the screen.

User Selected
![](000_Files/Pasted%20image%2020220912214816.png)
![](000_Files/Pasted%20image%2020220912214114.png)
- I create a function, the "boxstatus" function, specifically for changing the text of the window. It also logs the change in the "userdata.txt" file.

For there one, there is little graphical change, as all that is changed is the text as it runs through the voice command from the user. It also repeats in asking for voice input, unless the program is terminated.

**Graphics**
- The program features *very* *minimalistic* graphics. This is because I felt it would be too much of a challenge to use and improve on the basic Tkinter graphics. Furthermore, I feel the simplistic design of the logo makes up for the lack of visual dynamics and contrast in the graphical interface of the program. 
- I intended to use minimalistic graphics, as I believe that **the focus of a voice assistant should not be it's aesthetic beauty, but rather its functionality**. In using less engaging graphics, I hope that students will not be distracted by the program, and rather use the program to further improve their focus and productivity.

**User Interface**
- The user has 2 ways of interacting with the program:
	- Voice
		- The fundamental utility of the program is that one can use their voice to maximise the functionality of their computer usage. The program clearly indicates when it is listening for audio input, with the text box changing and an audio cue being played. 
	- Peripheral input (mouse)
		- For trivial things like starting the program and choosing an account, I decided to use Tkinter buttons for these things, as I felt they were not worth implementing voice commands, however for future designs of the program this should be implemented. 

- COMMENTS IN **ALGORITHM** CODE!!!
4. Develop
- See attached folder.
6. Test
- Trace table with **sample data**!!!
7. Evaluate
