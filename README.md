# mit-pei-website

Hey PEI! I'm editing the MIT PEI website here, using the Bootstrap "Mentor" Template (info at https://bootstrapmade.com/demo/Mentor/).

The home page of the website is the "index.html" file.
As you can see on the top left, the main branch is the "main" branch. This will be where all final updates/changes will be pushed for the final version of the website. I'll be making my edits/changes on my own branch, the "allygator" branch. It's good practice to do so this way so that if I ever mess up on my own branch, I always have the main branch's files saved on the cloud to revert to.

If you want to start editing the website or get the files on your computer, you can install git + link your Github on the Terminal and clone this repository onto your machine! More details on getting started would look something along these lines:

A good way to get started is this tutorial on Git/Github (https://youtu.be/SWYqp7iY_Tc). Here is also a cheat sheet of all the commands because there are so many, and it's nice to have at hand because it's better than memorizing everything haha: https://education.github.com/git-cheat-sheet-education.pdf.

After installing Git, making a Github account, and linking this account to your computer through Terminal (all shown in tutorial), *PLEASE LET ME KNOW YOUR GITHUB USERNAME, SO I CAN ADD YOU THE REPO SO YOU CAN COLLABORATE DIRECTLY ON THIS REPO.* 

Afterwards, you would clone the mit-pei-website repo, create your own branch, and edit the code! Before you initialize and clone the repo, make sure that you are in the folder you want these files to get replicated to.

You would check which folder you are in by typing `pwd` and pressing enter on the Terminal. The path should print out. My Terminal would look like this, for example:
```
(base) allygator@Gators-MacBook-Air mit-pei-website % pwd     #the command I typed
/Users/allygator/Desktop/                                     # the output, which is the path of my current folder
```
So I'm in Desktop. Right where I would want my "mit-pei-website" repo to be cloned!

To initialize and clone this repo, I would execute these commands on the Terminal:
```
git clone https://github.com/allymhong/mit-pei-website.git    # this link should be found at the top of the Github page, under the "code" button. I normally
                                                              # use the http address.
```

And finally, if you want to create your own branch to create edits:
```
git branch allygator                     # replace "allygator" with your desired branch name; this will create a new LOCAL branch
git checkout allygator                   # this command will let you switch your workspace to that branch.
                                         # all further staging ("git add") and committing ("git commit") would take place in this branch
git push origin allygator                # pushing my local branch to a remote "allygator" branch, creating a remote allygator branch to push to
```


Basically, Git/Github lets us keep track of all our work and all the varying versions. When we commit our changes, we can always see what edits/changes have been made in reference to the last committed version – and we can always revert to this as Git keeps track of our version history. Having varying branches also helps when we have multiple people working on the same code, so that we can compare our branches/versions and "merge" our work when finalizing our code.


So there are multiple levels of version control. When I edit any documents in the "allygator" branch, I'm making these edits locally in my working directory.

To add any changes to my files to the staging area, I would:
```
git add --all                           # could just be "git add index.html" or whichever file you made edits in, but I like to do this
                                        # so I don't have to type each file name individually
```

So for now, Git isn't actually keeping track of any versions yet. We are adding files to the staging area to get ready to fully commit these changes to a version of our branch; in other words, Git will not have records of our changes until we commit these files. I'm not completely sure why we even `git add` in the first place, but I think it's just to take a step before committing.

To commit, I would type:
```
git commit -m "changed title to PEI"    # so if you just typed "git commit", it would take you to some weird Terminal text editor
                                        # to avoid this, I normally type "git commit -m ________" with a message in string format that follows so that
                                        # this would be the explanation of my git commit. It's kind of annoying sometimes that git requrires us to commit
                                        # with a message, but it's good practice to always state what changes we made (esp. when looking back to where we made
                                        # a specific change we might want to reverse).
```

This is a good depiction of what's going on:
![Depiction of Git Add/Commit](assets/img/git.png?raw=true)


So finally! Our local git repository is tracking these committed changes/versions! How do I get these edits to my remote *GitHub* repository?
For that, we'd push our changes to the remote repository. Before we do so we might have to pull the most recent version of that remote repo.
```
git pull origin allygator               # make sure I have all the most recent version of the remote allygator branch
git push origin allygator               # push my version and changes to the remote allygator branch
```

It's also good practice to 
```
git fetch
```
every so often, which is how you make sure your local Git repo is keeping up with all the updated branches, commits, edits, etc. that your remote GitHub repo has. So if Marisa created a local AND remote branch "marisa", I wouldn't have access to these updates unless I `git fetch` this data.


Finally, when you're ready to make the big step by merging your branch into the main one, you would need to first checkout the main branch.
```
git checkout main                       # make sure you're on the main branch
git pull origin main                    # make sure you have the most recent version of the remote main branch
git merge allygator                     # merge the branch you've been working on to the main one! and it should work out fine unless there are conflicts within
                                        # merging, which should be figured out through GitHub
```

Thanks for reading thus far :) and sorry (again) for any confusions I may have caused from my wack tutorial lolol. The Git cheatsheet I linked to above should help with all of the functions necessary with Git! Thanks for reading :)
