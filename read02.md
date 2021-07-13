# **_Git_**
### befor talking about git we have to Know what is the Version Control

## **_Version Control:_**
Version Control is a system that allows you to go back and forth between different versions of a file or collection of files by keeping track of changes.

*Version control allows you to:*

1. You can go back to a prior version of a file or project.
2. maintaining a record of changes and modifying individuals
3. compare the changes
4. Mistakes in files may be easily rectified by utilizing a Version Control System (VCS).

## **_Version Control have three type:_**
### 1. Local Version Control:
A Local VCS entails one database on your hard disk that stores changes to files.
### 2. Centralized Version Control
This system entails a single server storing all changes and file versions, which can be accessed by various clients.
#### which helped to :
+ streamlined the collaboration process (by eliminating the need to involve all local databases).
+ allowed programmers to have more knowledge of team members’ activities with certain files.
+ gave administrators much more control over divvying up revision privileges.
### 3. Distributed Version Control
Its prevent  if the CVS goes down ,and lead to make  collaborators cannot work with each other on a file or save changes and new versions,which lead to a big problem so a DVCS allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information.Because the DVCS allows for multiple mirrored repositories, programmers working in teams can collaborate with each other in various ways to complete a joint project, which enables the use of various simultaneous workflows.

### **After this Introduction what is Git? **
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project `called commit `  you can add it throw  `git commit -m " add Message here "` then Git will creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

Git includes inherent Graphical User Interface (GUI) tools. but users can also utilize third-party tools created for particular platforms.

**GUI** mean **Graphical User Interface** or in other way " normal windows screen"

**CLI** mean **Command Line Interface** or in other way"The black screen terminal"

we can add commands  using Git the most popular commands are `add commit`,` puch origin main` which refer to `ACP`

- to add all file use `git add .`
- to see information regarding changes to be committed use `git status`
- to save the work with Message use `git commit -m "add Message here "`
- to push changes to a remote repository use `git push origin main`


