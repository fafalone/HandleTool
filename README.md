# HandleTool v2.0
List Files and other handles, find process using file

<img width="750" height="407" alt="image" src="https://github.com/user-attachments/assets/c4292395-eb7f-4d46-be4b-481fb8150060" />
<br>

<img width="657" height="329" alt="image" src="https://github.com/user-attachments/assets/329f7179-ca27-40cd-ae2d-89a502626763" />
<br>

<img width="303" height="199" alt="image" src="https://github.com/user-attachments/assets/2efc53c2-ed81-4a1a-9230-b7943e065fb5" />

<img width="323" height="178" alt="image" src="https://github.com/user-attachments/assets/893be36a-23a7-4368-a14a-90d037ec9dff" />

<br>
This is a small utility that lists files and several other (or all) handle types in use by a specified process. It also has a function to list all processes that have an open handle to a specified file (if the file can't be moved/deleted/etc because it's "in use", this will show the program(s) holding it open). 

 **Update (04 Dec 2025) - Version 2.0**
- Handles now in sorted ListView with multiple columns
- Option to close handle via right-click menu
- Option to kill process via right-click menu
- Additional categories for explicit handle types
- Token handles now look up domain\user as name
    
 **Update (04 Dec 2025) - Version 1.2**
- Enable SE_DEBUG_PRIVILEGE to be able to list/search for
   handles in SYSTEM processes.
- Fix NtPath->DosPath error in some cases from not mapping
    '  volumes on startup.
    
**Update (04 Dec 2025) - Version 1.1**
- Double click to list handles
- In some cases, NtQueryObject for the name would hang, so
     the name lookup is now done on a separate thread with a 
     250ms timeout.
- ListView should be single sel
- Section handle display broken
- Fixed some handle leaks
