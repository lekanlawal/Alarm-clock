from cgitb import text
from importlib.metadata import entry_points
import tkinter as tk
from tkinter import*
from tkinter import messagebox
from tkinter import*
import time, os
from playsound import playsound



os. system ("clear")

def widgets():

    label1 = Label(root, text= "Insert Time here in Hour:Minute - ")
    label1.grid(row =0, column =0, padx =5, pady =5)

    global entry
    entry = Entry (root, width=15)
    entry.grid(row =0, column =1)

    label2 = Label(root, text= " What do you want to be reminded about: ")
    label2.grid(row=1, column =0, padx =5, pady =5)

    global entry1
    entry1 = Entry (root, width=15)
    entry1 .grid(row =1, column =1)

    buttt = Button(root, text= "Enter", width=15, command= enter)
    buttt.grid(row=2, column=1)
    

    global label3
    label3 = Label (root,text ="")
    label3.grid(row=3, column=0)
    

def message1():

    global entry, label3
    Alarmtimelabel = entry.get()
    label3.config(text= "The Alarm has been set")
    messagebox.showinfo("Alarm Clock", f"Your Alarm will ring at: {Alarmtimelabel}")

def enter():

    global entry, entry1,label3
    Alarmtime = entry.get()
    message1()
    currenttime = time.strftime("%H:%M")
    alarmmessage = entry1.get
    print(f"The time for your Alarm is:{Alarmtime}")
    while Alarmtime != currenttime:
        currenttime= time.strftime("%H:%M")
        time.sleep(1)
    if Alarmtime == currenttime:
        print("IT'S ABOUT DRIVE, IT'S ABOUT POWER. STAY HUNGRY AND DEVOUR")
        playsound("/Users/lekanlawal/Downloads/Alarm-ringtone 2/Alarm-ringtone.mp3")
        label3.config(text= "Alarm Sound Playing")
        messagebox.showinfo("Alarm Message",f"Your Alarm set for {alarmmessage}")



root = tk.Tk()
root.title ("GLCT Alarm Clock ")
root.geometry("500x200")


widgets()



root.mainloop()
