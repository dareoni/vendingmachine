# vendingmachine

This code is an inventory management program that reads and processes data from JSON files representing inventory information for different locations. It calculates various statistics for each inventory item and provides a user interface to sort and display the items based on different criteria. Here's a breakdown of the code:

1. **InventoryItem Class** (`InventoryItem`):
   - Defines a class representing an inventory item.
   - Initializes an item with its name, total stocked quantity, total quantity in stock, and total slots.
   - Provides methods to add to the stocked and in-stock quantities, increment slots, get the number sold, sold percentage, stock need, name, and number in stock.
   - `__repr__` method returns a formatted string for displaying the item's statistics.

2. **Main Function** (`main()`):
   - Initializes a list of inventory file names (`inventoryFileNames`) representing different inventory locations.
   - Initializes an empty dictionary (`itemNameToInventoryItem`) to store `InventoryItem` objects with item names as keys.

3. **Reading and Processing Inventory Data**:
   - Loops through each inventory file name in the list.
   - Opens and reads the JSON data from the inventory file.
   - Extracts information about each slot (item) from the JSON data and updates the corresponding `InventoryItem` object in the dictionary.

4. **Sorting and Displaying Inventory Items**:
   - Provides a user interface loop that allows the user to sort and display inventory items based on different criteria.
   - The user can choose to sort by item name (`n`), percentage sold (`p`), stocking need (`s`), or quit (`q`).
   - Depending on the user's choice, the program sorts the list of `InventoryItem` objects (`inventoryItemsList`) accordingly and prints a formatted table displaying item statistics.

5. **Output Format**:
   - The program prints a formatted table showing each inventory item's name, number sold, sold percentage, number in stock, and stocking need.

6. **Running the Program**:
   - The `main()` function is called to run the inventory management program.

In summary, this code demonstrates a basic inventory management system that reads and processes inventory data from JSON files, calculates item statistics, and provides a user-friendly interface to sort and display the inventory items based on different criteria.
