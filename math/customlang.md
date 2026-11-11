In computer programming, there are often different structures by which we can represent programs. Generally, however, we have a few standard notions: being able to input data, being able to output data, being able to do computations/calculations with data, and being able to repeat code (i.e. do looping).

I have designed a language called rotelang which tries to capture these standard notions. In the language, I am basically mapping out the general structure of a program. We have a few symbols:

i = input data to the program. o = output data to the user. p = process data in the program. l = indicate the start of a loop. c = indicate the end of a loop.

Here, I present an example of how rotelang is used. Consider the following program in Python:

for i in range(10):
    base = input("Enter triangle base: ")
    height = input("Enter triangle height: ")
    area = base * height
    print("Area is " + str(area) + "square units.")
print("All done!")

In rotelang, we can represent this program as: lipoco. This is because we start a loop, get some inputs, process the data, output the data, close the loop, and output a closing message.

As practice, write a Python program which uses 2 for loops (one nested inside the other) to print all elements in the Cartesian product 2x5. Then, write rotelang for your program. The rotelang answer can be submitted as the password to access the protected file entries/rotelang_answer. Note: valid rotelang strings cannot be captured by a finite-state automaton.

### Answer

rotelang: llocc
