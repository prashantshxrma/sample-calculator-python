# python-sample-1
https://replit.com/@PrashantVashiis/app-for-assessment#app%20for%20assessment.py
import tkinter as tk

def calculate():
  try:
    result = eval(entry.get())
    output.config(text=f"Result: {result}")
  except:
    output.config(text="Invalid Input")

root = tk.Tk()
root.geometry("300x200")
root.title("Calculator")

entry = tk.Entry(root)
entry.pack()

button = tk.Button(root, text="Calculate", command=calculate)
button.pack()

output = tk.Label(root)
output.pack()

root.mainloop()

