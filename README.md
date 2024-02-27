import tkinter as tk

def login():
    # Add authentication logic here
    print("Logged in")

def open_guest_menu():
    # Add logic to open the guest menu window
    print("Opening guest menu")

# Window 1 Configuration
welcome_window = tk.Tk()
welcome_window.title("PizzaPal Express - Welcome and Login")

# Logo and Welcome Message
logo_label = tk.Label(welcome_window, text="PizzaPal Express Logo")
logo_label.pack()

welcome_label = tk.Label(welcome_window, text="Welcome to PizzaPal Express! Please log in.")
welcome_label.pack()

# Username and Password Entry Fields
username_label = tk.Label(welcome_window, text="Username:")
username_label.pack()

username_entry = tk.Entry(welcome_window)
username_entry.pack()

password_label = tk.Label(welcome_window, text="Password:")
password_label.pack()

password_entry = tk.Entry(welcome_window, show="*")  # Masking password
password_entry.pack()

# Login Button
login_button = tk.Button(welcome_window, text="Login", command=login)
login_button.pack()

# Guest Option
guest_button = tk.Button(welcome_window, text="Continue as Guest", command=open_guest_menu)
guest_button.pack()

welcome_window.mainloop()
