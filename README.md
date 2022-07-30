# How to edit markdown file click [here](https://github.com/ArpitB95/Documentation)

# Craeting-SSH-key
# Note: You must create your key in ssh directory and nowhere else,       because .ssh is hidden folder so it's more secure

- Open gitbash as an admin
-  enter command cd ~/.ssh, if you run this command it will take you to ~/.ssh directory.
-  If you have any error or don't have .ssh directory, you need to create one by using following command.
-  go to your main directory using cd command
-  then follow:
-   mkdir .ssh
-   cd .ssh  (to change directory to ssh)
-  
-   Now, to generate a new key run following command
-   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"  (change email       to your git email)

- After that it'll ask to name the key, name the key EX: 122 then enter
  Then it'll ask to put password, if you don't want to put password, leave   it blank and press enter.

- Then will ask to re enter password.( did'nt set up the password so again   leave it blank and press enter)
- Now it will create the footprint of the key
- Clear the screen
- ls
- you'll find the key with two files( in this example 122 and 122.pub)

- Now go to your git account 
- click on your profile > settings
- click on SSH and GPG keys
- click on new key 
- Name the key (Ex:122)
- Go to terminal 
- cat 122.pub
- copy the key ( make sure you copy only the key and not the blank spaces)
- Paste it in your git account 
- click on add SSH key

- Go to your terminal and enter cd .. (it will take you out of .ssh directory, you should never work in .ssh except creating a key)
