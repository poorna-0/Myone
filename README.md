def calculate_total(items):
    total = 0
   
    for item in items:
        total += item['price'] * item['quantity']
   
    return total


def generate_bill(items, total):
    print("\n************ Supermarket Billing System ************")
    print("---------------------------------------------------")
    print("Item\t\tQuantity\tPrice\t\tTotal")
    print("---------------------------------------------------")
   
    for item in items:
        print(f"{item['name']}\t\t{item['quantity']}\t\t{item['price']}\t\t{item['price'] * item['quantity']}")
   
    print("---------------------------------------------------")
    print(f"Total: {total}")
    print("---------------------------------------------------")


def supermarket_billing():
    print("WELCOME TO SUPERMARKET\n")
    print("Select a category:")
    print("1. Dairy Products")
    print("2. Groceries")
    print("3. Fruits & Vegetables")
    print("4. Dry Fruits")
    print("5. Electronics")
   
    category = int(input("Enter category number: "))
   
    items = []
   
    if category == 1:
        print("\nDairy Products:")
        print("1. Milk (1L) - 60/-")
        print("2. Curd (1/2L) - 30/-")
        print("3. Butter Milk (1Ps) - 15/-")
        print("4. Ghee (1/2kg) - 100/-")
        print("5. Butter - 150/-")
        print("6. Cheese - 200/-")
       
        while True:
            item = {}
            item_number = int(input("\nEnter item number (or 0 to quit): "))
           
            if item_number == 0:
                break
           
            if item_number < 1 or item_number > 6:
                print("Invalid item number. Please try again.")
                continue
           
            if item_number == 1:
                item['name'] = "Milk (1L)"
                item['price'] = 60
            elif item_number == 2:
                item['name'] = "Curd (1/2L)"
                item['price'] = 30
            elif item_number == 3:
                item['name'] = "Butter Milk (1Ps)"
                item['price'] = 15
            elif item_number == 4:
                item['name'] = "Ghee (1/2kg)"
                item['price'] = 100
            elif item_number == 5:
                item['name'] = "Butter"
                item['price'] = 150
            elif item_number == 6:
                item['name'] = "Cheese"
                item['price'] = 200
           
            item['quantity'] = int(input("Enter quantity: "))
            items.append(item)
           
    elif category == 2:
        print("\nGroceries:")
        print("1.Dal - 60/-")
        print("2. Oil (1L) - 180/-")
        print("3. Veniger (1L) - 50/-")
        print("4. Boost (1kg) - 200/-")
        print("5. Salt Packet - 30/-")
        print("6. Coffee Powder - 150/-")
       
        while True:
            item = {}
            item_number = int(input("\nEnter item number (or 0 to quit): "))
           
            if item_number == 0:
                break
           
            if item_number < 1 or item_number > 6:
                print("Invalid item number. Please try again.")
                continue
           
            if item_number == 1:
                item['name'] = "Dal(1 kg)"
                item['price'] = 60
            elif item_number == 2:
                item['name'] = "Oil(1L)"
                item['price'] = 180
            elif item_number == 3:
                item['name'] = "Veniger (1L) "
                item['price'] = 50
            elif item_number == 4:
                item['name'] = "Boost (1kg)"
                item['price'] = 200
            elif item_number == 5:
                item['name'] = "Salt Packet"
                item['price'] = 30
            elif item_number == 6:
                item['name'] = " Coffee Powder"
                item['price'] = 150
           
            item['quantity'] = int(input("Enter quantity: "))
            items.append(item)
           
    elif category == 3:
        print("\nFruits & Vegetables:")
        print("1.Apples(Kg) 180/-")
        print("2. Grapes(1Kg) 80/-")
        print("3. Orange(1Kg) 70/-")
        print("4. Water Melon 200-")
        print("5. Banana(12pcs) 60-")
        print("6. Kiwi(2pcs) 150/")
       
        while True:
            item = {}
            item_number = int(input("\nEnter item number (or 0 to quit): "))
           
            if item_number == 0:
                break
           
            if item_number < 1 or item_number > 6:
                print("Invalid item number. Please try again.")
                continue
           
            if item_number == 1:
                item['name'] = "Apples(Kg)"
                item['price'] = 180
            elif item_number == 2:
                item['name'] = " Grapes(1Kg)"
                item['price'] = 80
            elif item_number == 3:
                item['name'] = " Orange(1Kg) "
                item['price'] = 70
            elif item_number == 4:
                item['name'] = " Water Melon"
                item['price'] = 200
            elif item_number == 5:
                item['name'] = " Banana(12pcs) "
                item['price'] = 60
            elif item_number == 6:
                item['name'] = " Kiwi(2pcs)"
                item['price'] = 150
           
            item['quantity'] = int(input("Enter quantity: "))
            items.append(item)
           
    elif category == 4:
        print("\nDry Fruits:")
        print("1.Cashew(Kg) 800/-")
        print("2. Kismis(1Kg) 500/-")
        print("3. Pistha(Kg) 1700/-")
        print("4. Badam 1000-")
       
        while True:
            item = {}
            item_number = int(input("\nEnter item number (or 0 to quit): "))
           
            if item_number == 0:
                break
           
            if item_number < 1 or item_number > 4:
                print("Invalid item number. Please try again.")
                continue
           
            if item_number == 1:
                item['name'] = "Cashew(Kg) "
                item['price'] = 800
            elif item_number == 2:
                item['name'] = "Kismis(1Kg)"
                item['price'] = 500
            elif item_number == 3:
                item['name'] = " Pistha(Kg) "
                item['price'] = 1700
            elif item_number == 4:
                item['name'] = "Badam"
                item['price'] = 1000
           
            item['quantity'] = int(input("Enter quantity: "))
            items.append(item)
           
    elif category == 5:
        print("\nElectronics:")
        print("1.Fan 2800/-")
        print("2. Tube Light 300/-")
        print("3.Headsets 1700/-")
        print("4.Speakers 1000-")
       
        while True:
            item = {}
            item_number = int(input("\nEnter item number (or 0 to quit): "))
           
            if item_number == 0:
                break
           
            if item_number < 1 or item_number > 4:
                print("Invalid item number. Please try again.")
                continue
           
            if item_number == 1:
                item['name'] = "Fan "
                item['price'] = 2800
            elif item_number == 2:
                item['name'] = "Tube Light"
                item['price'] = 300
            elif item_number == 3:
                item['name'] = " Headsets "
                item['price'] = 1700
            elif item_number == 4:
                item['name'] = "Speakers "
                item['price'] = 1000
           
            item['quantity'] = int(input("Enter quantity: "))
            items.append(item)
    else:
        print("Invalid category number.")
    
    total = calculate_total(items)
    generate_bill(items, total)


supermarket_billing()
