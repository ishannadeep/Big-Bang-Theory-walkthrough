# Big-Bang-Theory-walkthrough
lets try to execute sheldon1 file. It says it is a bomb and we need to defuse it. If we type anything while the program running the bomb will explode. We must reverse engineer it to understand and defuse it. Type “gdb sheldon1” then type “info functions” to see the functions of the program.it has lot of them. Some of them are created specially for the program. Ex: secret_phase, explode_bomb, phase_defused, phase_1

![Capture](https://user-images.githubusercontent.com/22831322/76165167-c6f3eb00-617a-11ea-8db8-857d6a567776.PNG)

![Capture2](https://user-images.githubusercontent.com/22831322/76165180-f0ad1200-617a-11ea-8e94-be46a4f4e021.PNG)

![Capture3](https://user-images.githubusercontent.com/22831322/76165201-0de1e080-617b-11ea-9a01-8ff452038b31.PNG)

![Capture4](https://user-images.githubusercontent.com/22831322/76165210-2651fb00-617b-11ea-9453-a2153c5fc751.PNG)

![Capture5](https://user-images.githubusercontent.com/22831322/76165220-3ff34280-617b-11ea-8cf0-6f6d88792f8b.PNG)

Let’s see what inside the secret_phase. Type "disass secret_phase"

![Capture6](https://user-images.githubusercontent.com/22831322/76165264-9496bd80-617b-11ea-88e1-d86d1811e990.PNG)
 Now lets take a look at the another function called "phase_1".when disassemble it we can see the special memory location called "0x80497c0".If we print that value inside it in a string format we get "Public speaking is very easy.".now we need to insert this string after executing the program.

![Capture7](https://user-images.githubusercontent.com/22831322/76168656-ca499f80-6197-11ea-8392-ee02f1c4f7fd.PNG)

![Capture8](https://user-images.githubusercontent.com/22831322/76168694-04b33c80-6198-11ea-9d4a-8442d8199958.PNG)
