# dasharaquotes.github.io
import tkinter as tk
from tkinter import font

def create_quote_window():
    root = tk.Tk()
    root.title("Dashara Quotes")
    root.geometry("400x300")
    root.configure(bg="#f0f0f0")

    title_font = font.Font(family="Helvetica", size=16, weight="bold")
    quote_font = font.Font(family="Helvetica", size=12)

    title_label = tk.Label(root, text="Dashara Quotes", bg="#f0f0f0", font=title_font)
    title_label.pack(pady=10)

    quotes = [
        "Life is an experience, experiences never last.",
        "Opportunities missed may never pass in the same direction.",
        "People who do not give up on their dream are usually the most successful."
    ]

    for quote in quotes:
        quote_label = tk.Label(root, text=quote, bg="#f0f0f0", font=quote_font, wraplength=350)
        quote_label.pack(pady=5)

    root.mainloop()

create_quote_window()
