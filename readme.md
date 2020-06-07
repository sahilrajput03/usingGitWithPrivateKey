## This repo is to demonstrate the procedure to use multiple private keys in windows.

So, you all need to copy the config file and the required private keys(files), which you want to use on your system to the `c:\users\<userName>\.ssh\` directory. You can look up the the scheme how the demo two private keys are imported, and you may import as many as you want like that.

***

## Generate new key-

```bash
$ ssh-keygen -t rsa -b 4096 -C "sahilrajput03@gmail.com"
```

Step1: ^^ ABOVE COMMAND.  
//Use your own email address, this creates in your current working directory, when you do it with terminal.
//Also, remeber to name the file(by default it takes it as id_rsa), otherwise you'll need to rename it manually when you would need to save in the .ssh directory.
__

```bash
$ cat yourFile.pub | clip
```

Step2: ^^ABOVE COMMAND WILL COPY TO CLIPBOARD DIRECTLY.
Copy the content of .pub file(C:\Users\chetan\.ssh\something.pub) and paste it in Github>Settings>Ssh and Cpg keys>New Ssh key.