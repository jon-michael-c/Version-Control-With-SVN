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

![Screenshot from 2021-07-21 23-43-48](https://user-images.githubusercontent.com/53241212/126587354-50d3087e-ac5d-4910-8ae6-166af241e465.png)

Naviate to the trunk of the repo and you should see your contents from the server. You can start making changes and commits now.
`svn add` adds a file to be commited. Use `svn commit -m "MESSAGE"` to commit.

![Screenshot from 2021-07-21 23-50-02](https://user-images.githubusercontent.com/53241212/126587763-600380b5-f634-4531-808c-c14c6f40d165.png)
