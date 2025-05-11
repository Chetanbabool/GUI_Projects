import customtkinter as ctk

# Set appearance
ctk.set_appearance_mode("System")  # Modes: "System" (default), "Dark", "Light"
ctk.set_default_color_theme("blue")  # Themes: "blue" (default), "green", "dark-blue"

# Create app window
app = ctk.CTk()
app.title("Odd or Even Checker")
app.geometry("400x300")

# Function to check odd/even
def check_number():
    input_text = entry.get()
    try:
        number = int(input_text)
        if number % 2 == 0:
            result_label.configure(text="✅ It's an Even number", text_color="green")
        else:
            result_label.configure(text="🔹 It's an Odd number", text_color="blue")
    except ValueError:
        result_label.configure(text="❌ Invalid input. Please enter a valid integer.", text_color="red")

# Entry field
entry = ctk.CTkEntry(app, placeholder_text="Enter a number", width=200,height=50)
entry.pack(pady=(70,0))
# Button to trigger check
check_button = ctk.CTkButton(app, text="Check", command=check_number)
check_button.pack(pady=10)

# Result label
result_label = ctk.CTkLabel(app, text="", font=ctk.CTkFont(size=18))
result_label.pack(pady=20)

# Run the app
app.mainloop()
