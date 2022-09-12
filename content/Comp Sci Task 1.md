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
	- Furthermore, people who have used voice assistants before may demand high quality in graphical design of the program. Using Tkinter, I plan to provide a well-thought-out visual interface, however I have used copyrighted images (Siri logo) for parts of the visual design, as I feel its simplistic design fits my program.
- The program will fill its user's need for a simplistic, easy-to-learn voice assistant that will improve their productivity. It will also improve their quality of life, by helping its users achieve a healthy study schedule/routine.
- Having research many software licences, I have settled on using the MIT licence for my program. I believe this licence reflects my desires for the use of my program, as I hope that others can take the program and improve on it for their own use. I also believe that if their version of my voice assistant is both unique and helpful for others, that its developers should be able to relicense it.

**Licencing**
Currently, there are 3 main software licences used by companies across the world:
- *Permissive*
	- **Examples:**
		- BSD licences (family)
		- MIT Licence
		- Apache Licence
		- ISC Licence
		- JSON Licence
	- It is a kind of free-software licence, which means it is allows users to run the program the licence is attached to, analyse the code of the program, and most importantly redistribute modified version of the program under whatever licence fits. This essentially allows developers to configure a program how they see fit, and release their new program under a new licence.
	- Permissive licences are also very compatible with other licences, due to its minimal restrictions on the user.
	- *It should be noted that a crucial flaw with Permissive licences is that they do not guarantee the type of licence of derivative software, and thus can result in derivate programs that are not free or publicly available.*
	- There are a few requirements for users of a program under a permissive licence, if they wish to redistribute the software:
		- They must leave in the original copyright notice.
		- They must essentially retain the same style of licence as the original program. 
			- Essentially, any new software created from the initial software are as open-source as the original program.
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

**Resources:**
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




**Similar Products:**
- Alexa
	- Amazon's Alexa excels in its compatibility with many operating systems, such iOS and Android. It also has numerous unique commands, and even includes voice commands that can change settings. I have considered using voice-activated commands to change settings, but I feel there is simply not enough settings to change, and it would be redundant. Furthermore, as the program is a python file, it is generally incompatible with most computers, considering the amount of modules it relies on.
- Google Assistant
	- Google Assistant's greatest quality is its voice recognition software, which is some of the best in the world. However, through Google's text-to-speech module in Python, my voice assistant should have the same recognition capabilities. Stylistically, Google Assistant has a simplistic, colourful design, which I have been inspired by. The design of Google's voice assistant focuses on user interaction, in its friendly voice and extensive utility as a general assistant. I am able to use Google's text-to-speech via its Python module
- Siri
	- Apple's Siri is a very versatile voice assistant. It has limited settings, and is not very compatible compared to other well-known voice assistants. However, in terms of languages available, Siri is quite compatible, supporting up to 21 languages as of April 2021. Siri is mostly designed for mobile uses, which is why it is the most popular voice assistant for mobile devices. Unfortunately, as my program is written primarily in Python, and requires a lot of Python modules, it is incompatible for mobile use. However, I hope to design a voice assistant with much more basic voice commands than Siri, and my idea of customised voice commands give my program an advantage over Siri.
2. Plan and Design
- ==COMMENTS IN ALGORITHM CODE!!!==
4. Develop
- See attached folder.
6. Test
- Trace table with **sample data**!!!
7. Evaluate

