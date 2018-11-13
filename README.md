# 9.10

class ItemToPurchase:
    def __init__(self):
        self.item_name = "none"
        self.item_price = 0
        self.item_quantity = 0
        
    def print_item_cost(self):
        print(self.item_name + ' ' + str(self.item_quantity) + " @ $" + str(self.item_price) + " = $" + str( self.item_price * self.item_quantity ))
        

def main(): 
    print("Item 1")
    
    item1 = ItemToPurchase();
    
    item1.item_name = input('Enter the item name:')
    item1.item_price = int(input('\nEnter the item price:'))
    item1.item_quantity = int(input('\nEnter the item quantity:'))

    print("\n\nItem 2")
    
    item2 = ItemToPurchase()
    
    item2.item_name = input('Enter the item name:')
    item2.item_price = int(input('\nEnter the item price:'))
    item2.item_quantity = int(input('\nEnter the item quantity:'))
    
    print("\n\nTOTAL COST")

    item1.print_item_cost()
    item2.print_item_cost()
    
    total = (item1.item_price * item1.item_quantity) + (item2.item_price * item2.item_quantity)
    
    print("\nTotal: $" + str(total))
      
main()
