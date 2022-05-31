from cProfile import label
from cgitb import text
from tkinter import *
from tkinter import font

root = Tk()

def aumentar(): #botao +
  lb1 ['text'] + 1
  

def diminuir():
    lb1 ['text'] -1

root.grid_rowconfigure(0,weight=1)
root.grid_columnconfigure(0,weight=1)
root.grid_columnconfigure(1, weight=1)
root.grid_columnconfigure(2, weight=1)

bt1 = Button(root, text='-', font= 'arial 11')
bt2 = Button(root, text='+', font='arial 11')
lb1 = Label(root, text=0, font='arial 11')


bt1.grid(row=0, column=0, sticky=NSEW)
bt2.grid(row=0, column=2, sticky=NSEW)
lb1.grid(row=0, column=1, sticky=NSEW)



root.mainloop()
