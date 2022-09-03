# Learning-Git-Workshop
Performing various commands in git bash to know how remote sessions work  


ls or dir : for show the list of files and folder in current directory
clear or cls : for clear screen
cd : for change directory
cd .. : for go to previous directory
mkdir : for create new directory or folder
attrib +h +s +r : to hide any folder
attrib -h -s -r : to show any folder
ls -a : for see all hidden files too	
git init : initializes git reposetory
touch filename.txt : for creating new file 
git status : to check weather the change is saved or not
git add .(to add all file which are unsaved) or git filename.txt(for add specific file): to save changes
If authority identity is unkown, 
run : git config --global user.email "abcd@any.com"
    : git config --global user.name "something"
git commit -m "Hello" : to pass any message(for records - take picture)
git branch nameOfBranch : to create new branch(locally)
git branch : to see branches
git branch -r : to see all remote branches
git branch -a : to see all available branches(remotely or locally)
git branch -D nameOfBranch : to delete branch 
git checkout branch_name : to switch from current branch to branch_name
vi name.txt : to write some content inside new file 
	(press ctrl(may or not)+i to start writing and to stop writing press esc and then :x enter)
cat name.txt : to see the details written inside name
git restore --staged name.txt : to unsave any previously saved file
git reset IdcopiedFromLog : to clear log history above the copied Id
git log : to see entire history of the project
git stash : for not to save the history anywhere but to store at any different place from where we can get it back anytime
git stash pop : to get that thing back which is saved through stash
git stash clear : to clean or delete the things saved through stash
git remote add anyname(origin) URLofRepo(https://github.com/Ankit-34/First.git) : to attach repository URL with our project
	(In URL, First is the name of repository)
git remote -v : to see the URLs which are attached with the folder or project
git remote set-url origin URLOfNewRepo : to change repo from the same account
git push origin nameOfBranch(master) : to share the changes on URL
git push --all -f(for force push) : to push changes in repository
git pull upstream main : to see change in fork
git fetch --all(for all branches) --prune(deleted are also be fetched) : to fetch(take) all the comments
git reset --hard upstream/main : to reset the main branch of origin to the main branch of upstream
git clone URL(origine of particular project) : to download folders related to that project
git rebase -i IdcopiedFromLog : to merge comments
git config --global --list : to see the current account for pushing
git config --global user.name "your_username" : to chnage the global username
git config --global user.email "your_email_address@example.com" : to change to global email
git merge Branch_name : It will merge Branch_name with current branch
git reset --merge : to reset the merging of branch

Note:
1.Any folder that starts with our account, the name of that is going to be origin.
2.We directly can not make change in any others project, we need to fork for it.
3.From where we have forked the project, that URL is known as UpStream URL.
4.Commit means to save the change 

To push in new repo,
First open terminal in the folder which you have to push and run (git init) to initialize
Then (git add .) for add every file and folder to push in repo or (git add file_name.txt) to add one by one
Then run (git commit -m "Any message") for commit the changes
Then run (git branch -M branch_name(default main)) to select branch
Then run (git remote add origin link_of_the_repo_in_which_we_have_to_push) to connect to the repo remotely
Then (git push -u origin branch_name) to finally push all changes in repo

To push changes in existing repo,
git add .
git commit -m "Message"
git push
