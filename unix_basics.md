# Unix Basics

As previously mentioned, the server (aka other computer) is where the data is most likely going to be stored and analyzed. Now, this is a computer like any other, but the operating system is most likely different from what your computer uses; most computers have OS or Windows as the operating system, but most servers use an operating system called Unix/Linux (which are technically different, but the same for our purposes). To try to make this understandable to a non-computer person, OS and Windows are like an iPhone - there is a lot of easy-to-use, built-in functions that make it pretty easy to use but limits what you can do with it - and Linux is like an Android - you can customize a lot more and do a lot with it, but there is a bit more of a learning curve.

Luckily, you only need to know the very basics. That is, how to use the terminal to get to the necessary files and launch whatever programs you will use to analyze or view the data. With that being said, you can follow tutorial 1 & 2 only in this [Linux tutorial](https://www.ee.surrey.ac.uk/Teaching/Unix/) (but it is always better to do the rest - except tutorial 7, you can skip that).

## UNIX Tutorial for Beginners

There is always more helpful, useful information to learn about using Linux (aka the rest of the tutorial), but this covers the essentials. Regardless of if you chose to learn more, here are a couple of little helpful tips:

- When typing out a file path, if you use the tab button, it will autocomplete the directory/file name.
- If you add `&` after a command that launches a program with a GUI (aka a new window), it will allow you to continue to use the command line. Otherwise, you have to close the program before being able to use that terminal again (although you can always open up a new one).

It is also important to note that Unix has different shells (tcsh, bash, csh, etc.). They all do the same things essentially, but with different syntax. From what I have seen, bash and tcsh/csh seem to be the most common among neuroimaging programs.

# Not for beginners: These next parts are a bit more advanced and are put in here for later use.

## File Permissions

When you log onto a server being used by a research team, you will probably not be able to go into every folder or access every file. That is because each user on the server has certain permissions for what they can and cannot do.

So how do you know what files you do have access to? You can see that every file has it labeled when you use the command:
```
 ls -l /path/to/directory/you/want/to/view/contents/of
```

So what exactly does this scary output of random letters mean? [This article](https://linuxhandbook.com/linux-file-permissions/) gives a short and sweet description of how to read the permissions labels. In case you still had questions, [this article](https://www.guru99.com/file-permissions.html) gives more details on it.

You may hear or see the term “sudo privileges” or “root account.” Don’t fret, it’s not more scary terms to learn a lot about. The root account has all the privileges and access to everything. It’s like a landlord having a master key; they can go anywhere in the building and do anything they want (within reason). Having sudo privileges is a similar concept. Users can be given sudo privileges, which then allows them to do/access certain things that they may not have been able to without sudo privileges. It’s like being handed the master key for a task then giving it back.

## Transferring Files Between Servers

Using the Command Line: [This website](https://linuxize.com/post/how-to-use-scp-command-to-securely-transfer-files/) outlines how to transfer files between computers/servers with the command line. This is the fastest and most secure way to transfer files, and here are skeleton scripts for doing it:

### Transferring from your current server to another
```
scp -r /path/to/local/target/file {username}@{serveraddress}:/path/to/remote/target/directory
```
### Transferring from another server to your current server
```
scp -r {username}@{serveraddress}:/path/to/remote/target/file /path/to/local/target/directory
```
You will then be prompted to enter your password for the remote server and will see updates on the transfer progress printed to the command line.

**Note:** The `-r` tag is used to recursively copy the files; this must be done for directories in order to copy their contents.

**Example:** Transferring a directory from a different server to a local server:
```
scp -r johndoe1@imaginary.umd.edu:/home/bar /data/neurodev/foo/bar
```

Using Google Drive/Box are always options. You can open Google Chrome on the server using the command: `google-chrome`(this is just for the servers tha I use, it could also be another command such as`chromium`).

Ensure that you are not saving large amounts of data to your home directory. There is a low limit on how much data can be in your home directory at any given time, and if you go over that limit, then you can no longer use FastX to access the server. If this happens to you, you can use the command line to ssh into the server and remove files with the command:
```
rm -f /path/to/file
```
And directories with the command:
```
rm -rf /path/to/directory
```
Ensure to check invisible directories in your home directory. These are directories that do not typically show up when you use `ls` and typically start with a period (Ex. `/path/to/home/directory/.cache/`).

For transferring smaller files that you may need to search for, you can set up an SFTP session using an alternate application.

 - **Pros:** Easily interpretable file viewer (like on a standard computer), easy to use (point and click).

 - **Cons:** Slower, cannot transfer as large files. This is a good choice for small files that you may want to send back or switch quickly with ease, such as with tcsh/bash scripts. This can be easily done on mac or windows using an application such as Termius (which can also be used to interface with the server through the command line).

  <div align="center">
    <a href="viewing_data.md">Next Page - (Viewing Data/Drawing VOIs/Lesions)</a>
  </div>
 
<div align="center"; margin-top="10px">
  <a href="home.md">Home</a>
</div>

  <div align="center">
    <a href="what_is_neuroimaging_data.md">Last Page - (What is Neuroimaging Data)</a>
  </div>
