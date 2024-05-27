<p align="center">
  <b>Dynamic Groups in Azure AD and Microsoft 365</b>
</p>

Dynamic group membership adds and removes group members automatically using membership rules based on member attributes.

Login to Entra ID admin portal

<b>Groups</b> -> New Group -> Under Group type, Choose “Security”

<b>Group name:</b> Give it a name  - I named it a department name(HR_dept) because I want all employees in the HR department to be dynamically added to this group. 

Note: The employees are added to their department during user account creation. 

Group description: Put the description

<b>Membership type:</b> Choose “Dynamic user”

![DynamicG1](https://github.com/stahir131/Dynamic-Groups-in-Azure-AD-and-Microsoft-365/assets/64047385/10d0a4f9-7e7a-4a97-9974-2a7a04edadd7)

Select a group owner

Dynamic user members: This is where you make a query to add members to the dynamic group.

Click <b>“Add dynamic query”</b>

![DynamicG2](https://github.com/stahir131/Dynamic-Groups-in-Azure-AD-and-Microsoft-365/assets/64047385/19d57881-4745-4a66-b1a4-aa874b293d25)

Under  Configure Rules -> <b>“Property” </b> -> Choose “department”  

<b>Operator</b>  -> Pick “Equals” 

Value: Type HR

<b>Save</b><br />
<b>Create
</b>

![dynamicG3](https://github.com/stahir131/Dynamic-Groups-in-Azure-AD-and-Microsoft-365/assets/64047385/717cfe0d-877b-4a44-a7ec-4174a98bdde9)

I have created User1 and user2 who are HR employees and after a couple of minutes were dynamically added to the HR_dept group as seen below.

![dynamicG4](https://github.com/stahir131/Dynamic-Groups-in-Azure-AD-and-Microsoft-365/assets/64047385/684fb1ba-6b89-4de8-84a1-dc31828f539e)

