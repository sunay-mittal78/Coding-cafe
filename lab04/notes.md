What did --global mean here? What would happen if you left it out?
    --global means the name and email get saved for my whole user account, so every repository on this computer uses them. if i left it out it would only apply to the one repository i am inside, and it would not work at all outside a repo.
What appeared in ls -a but not in ls? What is inside it?
    a hidden folder called .git appeared (starts with a dot so plain ls skips it). it is where git keeps everything it knows about the repo, like the history of commits, the config and the branch info.
Roughly how many files and folders is Git offering to track? Does anything in that list look like something you did not write?
    git listed everything in the folder as untracked: README.md, week02, and the .venv/ folder. the .venv/ is the one i did not write, it is full of other peoples code (python and the requests package).
Compare this git status with the one from Question 3. What disappeared?
    .venv/ disappeared from the untracked list. git is now ignoring it because of the .gitignore, and .gitignore itself showed up in the list instead.
.gitignore itself shows up as untracked. Should it be committed, or ignored too? Why?
    it should be committed. it is a file i wrote and it is part of the project, so anyone who gets the repo should get the same ignore rules too. if it ignored itself the rules would stay only on my computer.
README.md moved from one heading to another in the git status output. Which two? In the three-places model from the session, what just happened to it?
    it moved from "Untracked files" to "Changes to be committed". in the three-places model it went from the working directory to the staging area.
What did Git print after the commit? How many files did it say changed?
    it printed the branch name with (root-commit), the short id of the commit and my message "Lab work so far". then a line saying [N] files changed with the number of lines inserted, and then the files that were created.
What are the first seven characters of your commit called, and what are they for?
    it is the short commit hash (a short version of the long id git gives every commit). it is used to name that exact commit, like when i want to look at it or go back to it.
You now have two commits. Without looking it up: what are the four steps of the loop you just did twice?
    git status to see what changed, git add to stage the file, git commit to save it with a message, and git log --oneline to check that the commit is in the history. (and before all this i edit the file.)
Why does this file get a special name and a special place, rather than being called notes.md like everything else?
    github looks for a file named README.md in the main folder of the repo and shows it on the front page. so it is the first thing anyone sees when they open the repo, and it explains what the project is.
What did gh auth login do that means you will not be asked for a password when you push?
    it logged me in to github through the browser and saved a login token on my computer. because i said yes to authenticate git, git uses that saved token every time i push, so it doesnt ask for a password.
Refresh the repository page on GitHub. What is showing on the front page, and why that file?
    my files and folders are showing, and below them the README.md displayed as formatted text with my name and roll number. it shows that file because github automatically displays the README.md as the front page of the repo.
Run git log --oneline again. Did pushing change your local history in any way?
    no, it looked the same, same commits in the same order. push only copies my commits to github, it doesnt change them. the only new thing is the label next to the latest commit showing origin/main.
Your repository is private but your TAs can now read it. In your own words, what is the difference between a repository being private and a repository not existing on GitHub at all?
    private means the repo does exist on github and is stored there, but only i and the people i invite (like the TAs) can see it. not existing means there is no copy online at all, so nobody could see it and i would have no backup.
