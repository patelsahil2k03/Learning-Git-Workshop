# Learning-Git-Workshop
Performing various commands in git bash to know how remote sessions work  


ls or dir : for show the list of files and folder in current directory <br />
clear or cls : for clear screen<br />
cd : for change directory<br />
cd .. : for go to previous directory<br />
mkdir : for create new directory or folder<br />
attrib +h +s +r : to hide any folder<br />
attrib -h -s -r : to show any folder<br />
ls -a : for see all hidden files too	<br />
git init : initializes git reposetory<br />
touch filename.txt : for creating new file <br />
git status : to check weather the change is saved or not<br />
git add .(to add all file which are unsaved) or git filename.txt(for add specific file): to save changes<br />
If authority identity is unkown, <br />
run : git config --global user.email "abcd@any.com"<br />
    : git config --global user.name "something"<br />
git commit -m "Hello" : to pass any message(for records - take picture)<br />
git branch nameOfBranch : to create new branch(locally)<br />
git branch : to see branches<br />
git branch -r : to see all remote branches<br />
git branch -a : to see all available branches(remotely or locally)<br />
git branch -D nameOfBranch : to delete branch <br />
git checkout branch_name : to switch from current branch to branch_name<br />
vi name.txt : to write some content inside new file <br />
	(press ctrl(may or not)+i to start writing and to stop writing press esc and then :x enter)<br />
cat name.txt : to see the details written inside name<br />
git restore --staged name.txt : to unsave any previously saved file<br />
git reset IdcopiedFromLog : to clear log history above the copied Id<br />
git log : to see entire history of the project<br />
git stash : for not to save the history anywhere but to store at any different place from where we can get it back anytime<br />
git stash pop : to get that thing back which is saved through stash<br />
git stash clear : to clean or delete the things saved through stash<br />
git remote add anyname(origin) URLofRepo(https://github.com/Ankit-34/First.git) : to attach repository URL with our project<br />
	(In URL, First is the name of repository)<br />
git remote -v : to see the URLs which are attached with the folder or project<br />
git remote set-url origin URLOfNewRepo : to change repo from the same account<br />
git push origin nameOfBranch(master) : to share the changes on URL<br />
git push --all -f(for force push) : to push changes in repository<br />
git pull upstream main : to see change in fork<br />
git fetch --all(for all branches) --prune(deleted are also be fetched) : to fetch(take) all the comments<br />
git reset --hard upstream/main : to reset the main branch of origin to the main branch of upstream<br />
git clone URL(origine of particular project) : to download folders related to that project<br />
git rebase -i IdcopiedFromLog : to merge comments<br />
git config --global --list : to see the current account for pushing<br />
git config --global user.name "your_username" : to chnage the global username<br />
git config --global user.email "your_email_address@example.com" : to change to global email<br />
git merge Branch_name : It will merge Branch_name with current branch<br />
git reset --merge : to reset the merging of branch<br />

Note:<br />
1.Any folder that starts with our account, the name of that is going to be origin.<br />
2.We directly can not make change in any others project, we need to fork for it.<br />
3.From where we have forked the project, that URL is known as UpStream URL.<br />
4.Commit means to save the change <br />

To push in new repo,<br />
First open terminal in the folder which you have to push and run (git init) to initialize<br />
Then (git add .) for add every file and folder to push in repo or (git add file_name.txt) to add one by one<br />
Then run (git commit -m "Any message") for commit the changes<br />
Then run (git branch -M branch_name(default main)) to select branch<br />
Then run (git remote add origin link_of_the_repo_in_which_we_have_to_push) to connect to the repo remotely<br />
Then (git push -u origin branch_name) to finally push all changes in repo<br />

To push changes in existing repo,<br />
git add .<br />
git commit -m "Message"<br />
git push<br />
