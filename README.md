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
git push allygator allygator             # pushing my local branch to a remote "allygator" branch, creating a remote allygator branch to push to
```


Basically, Git/Github lets us keep track of all our work and all the varying versions. When we commit our changes, we can always see what edits/changes have been made in reference to the last committed version – and we can always revert to this as Git keeps track of our version history. Having varying branches also helps when we have multiple people working on the same code, so that we can compare our branches/versions and "merge" our work when finalizing our code.

Hoping this tutorial was helpful >.< Please, please, please don't hesitate to reach out to me if you have any questions/comments/etc.! By next meeting, I wouldn't mind just walking through what I'm doing here too; I think it'd be better than these written instructions. Let me know! Happy coding, and happy holidays <3
