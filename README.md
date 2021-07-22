# Version Control With Subversion(SVN)
![external-content duckduckgo com](https://user-images.githubusercontent.com/53241212/126389284-d6fbe647-5b27-4bce-a132-1470354e652b.png)
SVN is a centralized version control system. It's different from distributed systems, like Git. Centralized version control means that the version history is stored in a central server. When a developer wants to make changes to certain files, they pull files from that central server to their own computer. After the developer has made changes, they send the changed files back to the central server.

# Configuring a SVN Repository
Setting up a repositority is similiar in nature to Git. First, you will need to set up a server to centralize the repository. Once you have a server, we must create a local repository within. Use `svnadmin create PATH_TO_DIRECTORY` to intialize. Type `svnserve -d -r PATH_TO_DIRECTORY` to activate the svn server.
\n

Server Terminal:

![Screenshot from 2021-07-21 23-03-22](https://user-images.githubusercontent.com/53241212/126584527-68f872c2-164c-4df8-bc06-f45b552006cb.png)

You should see these contents in the directory if completed sucessfully.

![Screenshot from 2021-07-21 23-05-42](https://user-images.githubusercontent.com/53241212/126584673-1281165f-b15e-4f32-a1e5-883250c26bde.png)

Now you can make another copy of the repository on a local machine. Use `svn checkout SERVER_ADDRESS` to pull the contents from the server.
\n

Local Machine:

![Screenshot from 2021-07-21 23-52-33](https://user-images.githubusercontent.com/53241212/126588759-96d42e3e-e40e-449f-bcf0-813feb0c3da4.png)



Naviate to the trunk of the repo and you should see your contents from the server. You can start making changes and commits now.
`svn add` adds a file to be commited. Use `svn commit -m "MESSAGE"` to commit.

![Screenshot from 2021-07-21 23-50-02](https://user-images.githubusercontent.com/53241212/126587763-600380b5-f634-4531-808c-c14c6f40d165.png)

Use `svn checkout` to put your changes to the server.

![Screenshot from 2021-07-21 23-43-48](https://user-images.githubusercontent.com/53241212/126588888-98dcac8e-7b1a-4cff-9f67-3339eaff1751.png)

If done sucessfully, you will see the changes on the sever.

Server Terminal:

![Screenshot from 2021-07-22 00-11-22](https://user-images.githubusercontent.com/53241212/126589012-1342a5b2-e3ad-4745-ae10-52fea95fb680.png)

# Comparison of Git and SVN commands
|Function|Git|SVN|
|:---|:---|---|
|  Documentation |https://git-scm.com/doc| https://svnbook.red-bean.com/
| Create new repository | git init | svnadmin create |
| Copy files to lcoal | git clone | svnadmin checkout|
| Commit changes | git commit | svn commit |
| Add a new file | git add | svn add | 
| Compare changes | git diff | svn diff |
