## Automate shutdown of all the Azure VM instances

1. Add user to Azure Active Directory __Application Developer role__.
2. Create a __Resource group__ and provide __loction__.
3. Search and Open ___Automation Account__.
   . Add __Automation Account__.
   . Provide __Name__,__subscription__,__Resource group__ name and __location__.
   . select Create __Azure Run As account__ yes.
   . select __create__.
4. Click on __created__ Automation Account
   . select __Start/Stop VM__ under __Related Resources__
   . From here, you can click __Learn more about and enable the solution__
   . In the __Start/Stop VMs during off-hours__ page for the selected solution, review the summary information and then click __Create__
5. On the __Add Solution__ page, select __Workspace__.select Create New Workspace. On the Log Analytics workspace page, perform the following steps.
  . Specify a name for __the new Log Analytics workspace__, such as "ContosoLAWorkspace".
  . Select a __Subscription__ to link to by selecting from the drop-down list, if the default selected is not appropriate.
  . For __Resource Group__, select an existing one.
  . Select a __Location__.
  . Select a __Pricing tier__. Choose the __Per GB (Standalone)__ option
6. After providing the required information on __the Log Analytics workspace__ page, click __Create__ 
   You can track its progress under __Notifications__ from the menu,which returns you to the __Add Solution__ page when done,
7. On the __Add Solution__ page, select __Automation account__
   . Provide VM Run book details.Specify the VM Exclude List (string). This value is the name of one or more virtual machines from the target resource group.
   . Provide date and time in __Shedule__.daily schedule will be created starting with the time that you selected
   . Provide Email details
   . click OK to close the __Parameters__ page and select __Create__ 

