# Revisions and the (C#)loud
---
## Git Out of Here!

Every aircraft contains what are known as 'black boxes'.  These boxes log every maneuver and input the pilots make on the aircraft.  Aircraft direction, speed, altitude and flightpath are all logged on the black box.  Data on the black box stores all of these inputs and may be viewed at future dates (e.g. there may be a mishap that requires investigation into the flight).

Git is the black box for programmers!  Fortunately for developers (and unfortunate for pilots) if a program crashes and burns, Git can load to a previous state (or snapshot) of their program and start again!  

Git allows developers to save snapshots and previous states of every single action.  Project teammates may see what lines of code were added or taken away, what functions were changed and how, or even leave comments for one another!

---
## Local Git <--> Cloud Git

Git works by having a main repository, or location, for your program.  This is then cloned to a local storage.  Once the clone is on the local storage, changes can be made that do not affect the main repository until the editor is ready.  Once the editor(s) is ready, they must remember and follow the workflow!

---

## Wax on, Wax off, Wax on...

### A C P 
The git workflow is represented by the acronym "ACP".  Add, Commit, Push.  

![Workflow](https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png)

For now, we will igore the pull and checkout actions in the photo above. 
1. Add - Add file to be tracked in the repo

2. Commit - file changed are commited along with a message that says what was changed

3. Push - File is pushed from the cloned local repository to the main repository that resides in the cloud!

---

### Read Between the Letters

Prior to 'add' you will have edited your actual file locally via VSCode or a similar text editor.  

Once added using git in terminal:

> git add filename.something

You will commit the changes with a message:

> git commit -m 'your message here'

Finally, we push!

>git push origin main

To check your status at any point, you can use the status command

> git status

Status will give you details such as how your local cloned repo matches up with the main repo.  It is useful to see what files have been changed and need to be committed and pushed to the main!


Get in terminal.  Practice these commands. You'll be a Git Giant in no time. 


~ QP3

[Home](../README.md)