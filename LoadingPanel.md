![panel_zaladunku](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/278f0a17-0e19-491f-b680-dd00fed0d69f)

Loading panel contains:
1. Top navbar (current shift, current data, todays output, refresh button)
2. Main table with last 100 orders
3. Add new order button
4. Edit selected order button
5. Check order button
6. Check material button
7. Selected couter

The main purpose of this panel is to facilitate operators' supervision over what is currently being painted and what has been painted. They can freely manipulate the order through panels for adding, editing, and deleting orders.

![dodawanie_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/d969ec53-1e12-4045-9358-649b65aa27b3)

Adding an order creates a new form for us, which, upon completion and clicking the green plus sign, adds a record to the database. Such a record is automatically assigned an ID number, a Primary Key, which allows the program to easily track specific records in the future and refer to them when needed.

![eydcja_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/6be36a90-5890-4950-aca0-95a1e0407032)

Editing begins by selecting the desired row and passing the data to a form that reproduces the order addition panel, but with the data from the selected row. In this panel, we can modify all the data, and then by clicking the green button, send the updated data to the database.

![usuwanie_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/b6d8bd89-e9c6-48cb-97a7-d17ebe80ade6)

To delete a record, you need to select the record and then press the delete button. As a precaution against accidental clicks, confirming the deletion is required in a popup window.

![przewodnik_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/082f87f8-fd17-42f0-80dc-4cb81d962fca)
![material_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/2bb91cbb-d2b3-4887-9362-486e0bae6779)

The last two options are used to search for a specific order or material in the entire database, and of course, after finding them, we can also edit them.

Workload:
Designing and creating a UML diagram ~5h
Creating main panel with all functions ~21h
Implementation ~2h
