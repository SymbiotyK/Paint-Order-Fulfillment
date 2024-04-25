![panel_zaladunku](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/030f24f7-3557-4a97-9965-dd3cc840769b)

Loading panel contains:  
1. Top navbar (current shift, current data, todays output, refresh button)
2. Main table with last 100 orders
3. Add new order button
5. Edit selected order button
6. Delete selected record button
7. Check order button
8. Check material button
9. Selected couter

The main purpose of this panel is to facilitate operators' supervision over what is currently being painted and what has been painted. They can freely manipulate the order through panels for adding, editing, and deleting orders.

![dodawanie_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/d969ec53-1e12-4045-9358-649b65aa27b3)

Adding an order creates a new form for us, which, upon completion and clicking the green plus sign, adds a record to the database. Such a record is automatically assigned an ID number, a Primary Key, which allows the program to easily track specific records in the future and refer to them when needed.

![eydcja_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/fa581c4f-edb5-463d-a36d-78735ad6731a)

Editing begins by selecting the desired row and passing the data to a form that reproduces the order addition panel, but with the data from the selected row. In this panel, we can modify all the data, and then by clicking the green button, send the updated data to the database.

![usuwanie_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/dada7f62-ea6f-4e0a-b07d-168a2751a8d8)

To delete a record, you need to select the record and then press the delete button. As a precaution against accidental clicks, confirming the deletion is required in a popup window.

![przewodnik_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/b650b880-1fff-4012-8cbb-ebf40a5ee43f)
![material_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/2bb91cbb-d2b3-4887-9362-486e0bae6779)

The last two options are used to search for a specific order or material in the entire database, and of course, after finding them, we can also edit them.

Workload:  
Designing and creating a UML diagram ~5h  
Creating main panel with all functions ~21h  
Implementation ~2h  
