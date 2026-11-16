What did pwd print?
    it printed the directory i am currently in

What did ls -a show that plain ls did not?
    .bash_history and other hidden files (the ones starting with a dot) that plain ls does not list, files that u cant normally see on File Explorer

Pick one line from ls -l. What do you think the first column means?
    "drwxr-xr-x" seems to be a code for what the item is and who is allowed to do what with it. 



Why does that work from where you are standing? Which kind of path is coding-cafe/week02? Absolute or Relative?
    its a relative path. it doesnt start with / so the terminal reads it starting from the folder i am currently in (home), and goes coding-cafe then week02 step by step


mv did two different jobs above. What were they?
    one was to move the file mentioned into the folder mentioned.
    then when i told it to move it into a file that didnt exist, it practically created a new file with the name and moved the data into the new file:
    essentially renaming the old file with the name given.


How many folders are on your PATH? (They are separated by :)
    way to many. Windows, Games, C drive, users.... 17 folders


Write down exactly where your python3 lives. You will need this again in a minute.
    /usr/bin/python3


Compare your answer to 7 with the person next to you. Are they the same? If not, why might that be?
    (doing the assignment alone in the common room) it might not as everyones path may differ. the location where python downloaded for me might be different for them + mac vs windows difference will also be there.


What exactly did the shell say? Explain the error in your own words, using the word PATH.
    it said "pyton3: command not found". the shell went through all folders on the PATH looking for something called pyton3 and found nothing, because that name doesnt exist.


.venv did not appear with plain ls. Why not? (Refer back to section 1.)
    because the name starts with a dot, so its a hidden folder. plain ls skips hidden stuff and ls -a shows it, same as .bash_history in Q1.

What changed about your prompt?
    (.venv) showed up at the very start of the prompt, before the path and whatever i type into the prompt.
    
Compare this with what you wrote down for question 7. Is it the same path? If not, what does that tell you about what activate actually did to your PATH?
    not the same. now it points to the python3 inside the .venv folder (/home/sunay_mittal/coding-cafe/.venv/bin/python3) instead of /usr/bin/python3. I have no idea what that means - maybe only the virtual environment is looked at first or only that is looked at and not the global enviornment


What is in the second list that was not in the first?
    requests showed up, along with the other packages it donwloaded to work with (urllib3, idna, certifi, charset-normalizer). the first list only had the basic stuff like pip that was pre-installed with venv.

    
Where does python3 point now?
    back to /usr/bin/python3, same as before the venv. deactivate took .venv/bin back off the PATH.

    
Find what ls -h does. Write it in your own words.
    it makes the file sizes human readable. used with -l, it shows sizes like 4.0K or 1.2M instead of a long number of bytes.


What is the difference between what Ctrl + C and Ctrl + D did?
    ctrl+c stopped python, it printed KeyboardInterrupt and python was still open. ctrl+d closed python completely and took me back to the normal terminal prompt.
