# Paint-Order-Fulfillment (DONE)
An application based on the Microsoft Power Apps low-code environment to manage and analyze orders on a painting line.
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
The application was built on the Microsoft Power Apps platform and deployed on the Teams platform, allowing operators to easily input painting orders along with technological data. Through integration with SharePoint List, order data is automatically stored and processed, enabling the generation of periodic reports and analyses. The creation of the application stemmed from the lack of a process reporting system, which made it difficult to conduct in-depth analysis of order flow.

Features:
- Loading panel: the main panel where orders are input when they enter the painting department.
- Unloading panel: used to input "Not OK" (NOK) pieces and mark those needing sandblasting.
- Sandblasting panel: tracks NOK pieces previously marked in the unloading panel, allowing operators to assign them sandblasting dates and tag numbers since identification labels are removed from blocks, and such tagging helps in their later retrieval.
- Analysis panel for the technologist.

Technologies used:
- MS Teams as the primary platform for launching the application and storing data.
- SharePoint Lists as the database.
- Excel for creating dynamic reports and analyses.

Workload:  
Designing and creating a UML diagram ~5h  
Creating all panels with functionality ~42h  
Implementation ~3h  
