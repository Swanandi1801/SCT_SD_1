print("=== Temperature Converter ===")
print("1. Celsius to Fahrenheit")
print("2. Celsius to Kelvin") 
print("3. Fahrenheit to Celsius")
print("4. Fahrenheit to Kelvin")
print("5. Kelvin to Celsius")
print("6. Kelvin to Fahrenheit")

choice = input("\nPick your conversion (1-6): ")
temp = float(input("Enter temperature value: "))

if choice == "1":
    result = (temp * 9/5) + 32
    print(f"{temp}°C = {result:.1f}°F")
    
elif choice == "2":
    result = temp + 273.15
    print(f"{temp}°C = {result:.1f}K")
    
elif choice == "3":
    result = (temp - 32) * 5/9
    print(f"{temp}°F = {result:.1f}°C")
    
elif choice == "4":
    celsius = (temp - 32) * 5/9
    result = celsius + 273.15
    print(f"{temp}°F = {result:.1f}K")
    
elif choice == "5":
    result = temp - 273.15
    print(f"{temp}K = {result:.1f}°C")
    
elif choice == "6":
    celsius = temp - 273.15
    result = (celsius * 9/5) + 32
    print(f"{temp}K = {result:.1f}°F")
    
else:
    print("Please pick a number from 1-6!")

print("\nDone!")

