# Version Control With Subversion(SVN)
![external-content duckduckgo com](https://user-images.githubusercontent.com/53241212/126389284-d6fbe647-5b27-4bce-a132-1470354e652b.png)
SVN is a centralized version control system. It's different from distributed systems, like Git. Centralized version control means that the version history is stored in a central server. When a developer wants to make changes to certain files, they pull files from that central server to their own computer. After the developer has made changes, they send the changed files back to the central server.

# Configuring a SVN Repository
Setting up a repositority is similiar in nature to Git. First, you will need to set up a server to centralize the repository. Once you have a server, we must create a local repository within. Use `svnadmin create PATH_TO_DIRECTORY` to intialize. Type `svnserve -d -r PATH_TO_DIRECTORY` to activate the svn server.
\n

Server Terminal:

![Screenshot from 2021-07-21 23-03-22](https://user-images.githubusercontent.com/53241212/126584527-68f872c2-164c-4df8-bc06-f45b552006cb.png)

You should see these contents in the directory if completed sucessfully

![Screenshot from 2021-07-21 23-05-42](https://user-images.githubusercontent.com/53241212/126584673-1281165f-b15e-4f32-a1e5-883250c26bde.png)

Now 
