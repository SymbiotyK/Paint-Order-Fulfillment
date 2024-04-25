![panel_zaladunku](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/278f0a17-0e19-491f-b680-dd00fed0d69f)

Loading panel contains:
1. Top navbar (current shift, current data, todays output, refresh button)
2. Main table with last 100 orders
3. Add new order button
4. Edit selected order button
5. Check order button
6. Check material button
7. Selected couter

Główny cel tego panelu to ułatwienie operatorm nadzór nad tym co jest aktualne malowane i co zostało pomalowane, mogą dowolnie manipulować zleceniem poprzez panele do dodawania zlecenie, edycji zlecenia i usuwania zlecenia.

![dodawanie_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/d969ec53-1e12-4045-9358-649b65aa27b3)

Dodwanie zamówienia tworzy nam nowego formsa który po wypełnieniu i kliknięciu zielonego plusika dodaje record do bazy danych, taki record ma nadawany automatycznie numer ID, Primary Key, dzięki któremu w przyszłoci program może łatwo śledzić konkretny record i odwoływał się do niego w rządanej chwili.

```
Patch(
    'Paint Order database';
    Defaults('Paint Order database');
    { 
        Tytuł: DataCardValue1_2.Text;
        material_num: DataCardValue2_2.Text; 
        load_date: DateValue1_2.SelectedDate + Time(Value(HourValue1_2.Selected.Value);Value(MinuteValue1_2.Selected.Value);0); 
        pc_count: Value(DataCardValue3_2.Text);
        double_pass: DataCardValue4_2.Value;
        comment: DataCardValue5_2.Text;
        shift: DataCardValue8_2.Selected.Value
    }
);;
Navigate(loadingservicescreen;ScreenTransition.Cover);;
ResetForm(Addform)
```

![eydcja_zaladunek](https://github.com/SymbiotyK/Paint-Order-Fulfillment/assets/161228121/6be36a90-5890-4950-aca0-95a1e0407032)

Edycja zacztuje wyselectowany wiersz i przekazuje dane do formsa który odtwarza panel do dodwania zlecenia z tym że z danymi z wiersza. W tym panelu możemy zmienić wszystkie dane a następnie klikając zielony przycisk wysłać aktualne dane do bazdanych.
