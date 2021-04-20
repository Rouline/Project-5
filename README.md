# Project-5
print("   CANADIAN SPACE AGENCY, CSA   ")
print()

menu = {}
menu['C']="Celcius"
menu['F']="Fahrenheit"
menu['K']="Kilometer"
menu['NM']="Nautical_miles"
menu['ML']="Miles"
menu['KM']="Kilometer"
menu['M']="Meter"
menu['CM']="Centimeter"
menu['M2']="Meter"
menu['Y']="Yard"
menu['CM2']="Centimeter"
menu['IN']="Inches"
menu['E']="Exit"
while True:
    options=menu.keys()

    for entry in options:
        print (entry, menu[entry])
    option=input("Please select:")
    if option == 'C':
        #convert from Fahrenheit to Celsius
        temp = float(input("Enter temperature in Fahrenheit: "))
        celsius = (temp - 32)*5/9
        print(f"{temp} in Fahrenheit is Equal to {celsius} in Celsius")        
    elif option =='F':
        #convert from celsius to fahrenheit
        celsius = float(input("Enter temperature in Celsius"))
        fahrenheit=(celsius * 9/5) + 32
        print("%.3f Celsius is: %0.3f Fahrenheit" %(celsius, fahrenheit))
    elif option =='K':
        #convert Nautical miles to Kilometers
        nautical_miles = float(input("Enter the value in Nautical Miles: "))
        kilometers=nautical_miles * 1.852
        print('%0.3f  miles is equal to %0.3f kilometers' %(nautical_miles, kilometers))
        print("%.3f Celsius is: %0.3f Fahrenheit" %(celsius, fahrenheit))
    elif option =='NM':
        #convert Kilometers to Nautical miles
        kilometers = float(input("Enter the value in Kilometers: "))
        nautical_miles = kilometers / 1.852
        print('%0.3f  kilometers is equal to %0.3f nautical_mile' %(kilometers, nautical_miles))
    elif option =='ML':
        #convert kilometers to miles
        kilometers = float(input("Enter value in kilometers: "))
        miles=kilometers / 1.609
        print('%0.3f kilometers: %0.3f miles' %(kilometers, miles))
    elif option =='KM':
        #convert miles to kilometers
        miles=float(input("Enter the value in miles: "))
        kilometers=miles * 1.609
        print("%0.3f  miles: %0.3f kilometers" %(miles, kilometers))
    elif option =='M':
        #convert centimeter to meter
        centimeter = float(input("Enter the Value Centimeter"))
        meter=centimeter / 100
        print("%.3f Centimeter: %0.3f Meter" %(centimeter, meter))      
    elif option =='CM':
        #convert meter to centimeter
        meter= float(input("Enter the Value Meter"))
        centimeter=meter * 100
        print("%.3f Meter: %0.3f Centimeter" %(meter, centimeter))
    elif option =='M2':
        #convert yard to meter
        yard = float(input("Enter the Value in Yard: "))
        meter=yard / 1.094
        print("%.3f Yard: %0.3f Meter" %(yard, meter))
    elif option =='Y':
        #convert meter to yard
        meter = float(input("Enter the Value in Meter: "))
        yard=meter * 1.094
        print("%.3f Meter: %0.3f Yard" %(meter, yard))        
    elif option =='CM2':
        #convert inches to centimeter
        inches=int(input("Enter the value in Inches:"))
        centimeter=inches*2.54
        print("%.3f Inches: %0.3f Centimeter" %(inches, centimeter))
    elif option =='IN':
        #convert centimeter to inches
        centimeter=int(input("Enter the value in Centimeter:"))
        inches=centimeter/2.54
        print("%.3f Centimeter: %0.3f Inches" %(centimeter, inches))
    elif option =='E':
        break       
    else:
        print("invalid option")
print("Thanks for using this programme. Goodbye")
