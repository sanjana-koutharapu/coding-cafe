\# Lab 1 - The Terminal



\## Section 1



\### Q1. What did pwd print?



`C:\\Users\\sanja`



\### Q2. What did ls -Force show that plain ls did not?



`ls -Force` did not show anything extra compared with plain `ls` in my current directory. Both commands showed week01, week02, and README.md.



\### Q3. Pick one line from ls. What do you think the Mode column means?



The Mode column shows the type and attributes of an item. For example, `d-----` indicates that the item is a directory.



\## Section 2



\### Q4. Why does ls coding-cafe\\week02 work from where you are standing? Which kind of path is coding-cafe\\week02, absolute or relative?



It works because the path is being interpreted starting from my current directory. `coding-cafe\\week02` is a relative path because it does not start from the root of the drive.



\## Section 3



\### Q5. mv did two different jobs above. What were they?



The first `mv` moved `README-backup.md` from the `coding-cafe` folder into the `week01` folder. The second `mv` renamed `README-backup.md` to `old-readme.md` while keeping it in the same folder.



\## Section 4



\### Q6. How many folders are on your PATH?



There are 10 folders on my PATH.



\### Q7. Write down exactly where your python lives - the Source column.



The Source column showed:



`C:\\Users\\sanja\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe`



\### Q8. Compare your answer to 7 with the person next to you. Are they the same? If not, why might that be?



My answer may be different from the person next to me because Python can be installed in different locations on different computers. The PATH is also specific to each computer and user.



\### Q9. What exactly did the shell say? Explain the error in your own words, using the word PATH.



The shell said that `pyton` was not recognized as the name of a cmdlet, function, script file, or executable program. This happened because `pyton` was misspelled, so PowerShell could not find that command on my PATH.



\## Section 5



\### Q10. .venv did not appear with plain ls. Why not?



In my terminal, `.venv` actually appeared with plain `ls`, so the expected hidden-file behavior described in the question did not occur. `ls -Force` also showed `.venv`.



\### Q11. What changed about your prompt?



The prompt changed by adding `(.venv)` at the beginning. This shows that the virtual environment has been activated.



\### Q12. Compare this with what you wrote down for question 7. Is it the same path? If not, what does that tell you about what Activate.ps1 actually did to your PATH?



The path is different from the one I recorded in Q7. Before activation, Python pointed to `C:\\Users\\sanja\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe`, but after activation it points to `C:\\Users\\sanja\\coding-cafe\\.venv\\Scripts\\python.exe`. This shows that Activate.ps1 changed the PATH so that the virtual environment's Python is found first.



\### Q13. What is in the second list that was not in the first?



The second list contains `requests` and its dependencies, which were not in the first list. These are `certifi`, `charset-normalizer`, `idna`, `requests`, and `urllib3`.



\### Q14. Where does python point now?



After deactivating the virtual environment, Python points to `C:\\Users\\sanja\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe`. This is the same Python path that I recorded in Q7.



\## Section 6



\### Q15. Find what the -Recurse flag does. Write it in your own words.



The `-Recurse` flag tells PowerShell to include items inside subdirectories when performing a command. Instead of stopping at the current directory, it goes through the directory tree below it.



\## Section 7



\### Q16. What is the difference between what Ctrl + C and Ctrl + Z did?



Ctrl + C interrupted the running Python process. Ctrl + Z followed by Enter sent the end-of-input signal on Windows, ending the input to the program.

