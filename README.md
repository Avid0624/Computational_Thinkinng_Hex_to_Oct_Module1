# Computational_Thinkinng_Hex_to_Oct_Module1
This is for an assignment in my computational thinking class. 
#hex_num = input("Enter a hexidecimal number: ")

try:
# Step 1: Convert the hexidecimal string to its decimal (integer) equivalent.
 # The int() function takes the string and the base (16 for hex) as arguments.
 dec_num = int(hex_num, 16)

 # Step 2: Convert the decimal number to its octal string representation.
 # The oct() function returns a string prefixed with '0o'.
 oct_num_with_prefix = oct(dec_num)

 # Step 3: Remove the '0o' prefix from the octal string using slicing. 
 #Slicing [2:] starts the string from the character at index 2.
 oct_num = oct_num_with_prefix[2:]

 # Display the final converted octal number.
 # The following is a descriptive text format for the output. 
 print(f"The octal equivalent of '{hex_num}' is: {oct_num}")

 except ValueError:
 # Handle cases where the input is not a valid hexadecimal number.
 # The following is a descriptive text format for the error message.
 print("Invalid input. Please enter a valid hexadecimal number (0-9, A-F).")

 
