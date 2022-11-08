# LEARNING GIT (GIT_NOTES)

Folder (Windows) --> Directory (Linux) --> Repository (Git) <br>
## Configuring username and email
`git config --global user.name ‘zainab-Memon’` <br>
`git config --global user.email ‘zainabsafi23@gmail.com’`

## Go to the folder where you want to initialize the git (track the folder) 
1. Open Git Bash in the folder/directory you are present in and enter following command: <br>
`git init` <br> 
*Note: Any file that starts with a dot(.) is a hidden file in linux* <br> <br>
2. Check the state of your files or stage of your files with this command: <br>
`git status` <br>

### States of Files in Working Directory
Every file in the working directory has 2 states: <br>
- Untracked  
- Tracked <br>
		- Unmodified <br>
		- Modified <br>
		- Staged <br>
3. Now, track the unmodified or new files  with this command: <br>
`git add` <br>
To add single file, run: <br>
`git add <filename>` <br>
To add all files, run: <br>
`git add .`

4. Now if we modify the file, the status will show the modified stage, you have to track the file again by using: <br>
`git add` <br>
Now the file will be in staged state
5. Commit The Changes <br>
Now after staging the file, you have to commit the changes, it will take snapshot and store the file in .git folder
You must store a msg with commit command for future use, to remember the reason you had made change or what changed did you make in the files.  <br>
`git commit –m “message in quotes”` <br>
- Note: If you run: `git commit` then a text editor, by default VIM is opened where you can make changes. VIM is **difficult for beginners** to use, especially, if you do not have any Linux/Unix exposure.So, it is better to change it to some other editor, like VScode.<br>
Following command changes the editor to VScode: <br>
`git config --global core.editor "code --wait"`
6. Check the logs <br>
It shows the logs and history of all of your commits that you make throughout your journey. Run:
`git log`
## Summary
- Configuring username and email <br>
`git config --global user.name ‘name’`
`git config --global user.email ‘abc@fxyz.com’` 
- Initializing Repository <br>
`git init` 
- Adding Files in Staging Area <br>
`git add` 
- Removing Files in Staging Area <br>
`git reset HEAD --` 
- Committing <br>
`git commit`
- Checking Current Status <br>
`git status`
- Checking Logs <br>
`git log`
