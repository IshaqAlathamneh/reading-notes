***Git tutorial***

In order to explain Git, we have to first explain various aspects of Version Control.

**What is the Version Control?**

Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes.

**Types of Version Control**
* Local Version Control
  * A Local VCS entails one database on your hard disk that stores changes to files.
* Centralized Version Control
  * This system entails a single server storing all changes and file versions, which can be accessed by various clients.
  * This proccess allowed programmers to have more knowledge of team members’ activities with certain files, and gave administrators much more control over divvying up revision privileges.
* Distributed Version Control
  * To prevent any type of catastrophic loss, a DVCS allows clients to create mirrored repositories. 
  * The data backups can be easily be placed on the server to replace any lost information.
  
**So, what is Git?**

1. Snapshots
   1. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it.
1. Local Operations
   1. Git mostly relies on local operations because most necessary information can be found in local resources.
1. Tracking Changes 
   1. Every single change applied to any file or directory is tracked by Git. 
   1. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.
1. Loss of Data
   1. Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data.
1. States 
   1. Committed: Data is securely stored in a local database
   1. Modified: File has been changed but not committed to the database
   1. Staged: Flagged a file’s changed version to be committed in the next snapshot

**Download Git**

[Mac OS](http://git-scm.com/download/mac)

[Windows](http://git-scm.com/download/win)

[Linux](http://git-scm.com/download/linux)

**More features:** You can import an existing project or directory into Git or You can also create a copy of an existing Git repository and you can get Help.

**Local Repository Structure**
1. Working Directory: The actual files reside here.

1. Index: The area used for staging

1. Head: Points to the most recent commit

**Saving Changes** 

* Tracked: Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

* Untracked: Untracked files were not in the last snapshot and do not currently reside in the staging area.

**The Life Cycle of File Status**

1.After you edit a file, Git flags it as modified because of changes made after the previous commit.

1.You stage the modified file.

1.Then, you commit staged changes.

**Remote Repositories**

In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network.

*Cloned Repositories*

For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

*Seeing Your Remotes*

By running the `git remote` command, you can view the short names, such as “origin,” of all specified remote handles.

By using `git remote -v`, you can view all the remote URLs next to their corresponding short names.
