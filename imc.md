from tkinter import *

#window
mc=Tk()
def somar():
   r=(float(in2.get())) / ((float(in1.get()))*(float(in1.get())))

   if r < 18.5:
    lb4['text']='Peso Baixo'
   if r >18.5 and r<24.9:
    lb4['text']='Peso Normal'
   if r >24.9 and r<29.9:
    lb4['text']='Sobrepeso'
   if r >30.0 and r<35.0:
    lb4['text']='Obesidade 1'
   if r >35.0 and r<40.0:
    lb4['text']='Obesidade 2'
   if r >=40.0:
    lb4['text']='Obesidade 3'
#widgets
lb1= Label(mc, text='Cálculo MC', font='Arial 20')
lb2= Label(mc, text='Altura', font='Arial 20')
lb3= Label(mc, text='Peso', font='Arial 20')
lb4= Label(mc, text='Status', font='Arial 16')
in1=Entry()
in2=Entry()
bt1= Button(mc, text='Calcular', font='Arial 20', command=somar)

#layout
lb1.grid(row=1,column=0, padx= 10, pady=10)
lb2.grid(row=2,column=0, padx= 10, pady=10)
in1.grid(row=3,column=0, padx= 10, pady=10)
lb3.grid(row=4,column=0, padx= 10, pady=10)
in2.grid(row=5,column=0, padx= 10, pady=10)
bt1.grid(row=6,column=0, padx= 10, pady=10)
lb4.grid(row=7,column=0, padx= 10, pady=10)

#run
Tk=mainloop()
