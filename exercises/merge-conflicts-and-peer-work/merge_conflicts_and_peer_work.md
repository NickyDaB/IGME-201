# Participation: Merge Conflicts and Peer Work

## Goal
Practice another component of version control, dealing with a merge conflict and collaborating with another teammate.

## Instructions

### Setting Up

Before we get to the important parts of the exercise that we want to practice. We need to set up our environment. 

Partner A should go to your GitHub profile and make a new repo. Name it "merge-conflicts-and-peer-work". Make it public. Add a README file. Leave gitignore and license as none.

Partner B won't be making a repo for this particular exercise.

This shouldn't be new, since we have done this in the last few exercises, but if you have issues, then raise your hand and ask Nick for help or ask your teammate for this exercise. Remember good collaboration is key!

![screenshot](1.png)

Once the repository is created, we need Partner A to add Partner B as a collaborator. 

Go to the settings of your newly created repo.

![screenshot](2.png)

Find "Collaborators" on the left navigation bar.

![screenshot](3.png)

This will bring you to a new sub-page called "Collaborators and teams" and this is one way to have multiple people work on the same project and repository. 

![screenshot](4.png)

This is probably a good name for this because a collaborator is someone who a who works jointly on an activity or project. Wow! Learning vocabulary! Look at us. :) 

Now, in order to work with our partner we will need to add them as a collaborator on this repo. Partner A should click on the "Add people" button.

![screenshot](5.png)

Search by your partner's username and invite them to the repo.

![screenshot](6.png)

![screenshot](7.png)

![screenshot](8.png)

After Partner A adds Partner B to the repo, you should see a "pending invite" status in the manage access list. 

![screenshot](9.png)

Partner B should recieve and email or some sort of notification. Accept it and become a collaborator on this repo. When partner B does this, the pending invite status should update.

![screenshot](10.png)

### Getting to work

Now each partner should clone the repo down to your local machine using GitHub Desktop. When you have done this your local folder, GitHub Desktop, and github.com should look similar to these states:

local folder:

![screenshot](11.png)

GitHub Desktop:

![screenshot](12.png)

github.com:

![screenshot](13.png)

Now partner A should go into the local folder and create a new file called `demo.txt`.

![screenshot](14.png)

Inside that file, Partner A should write the following lines.

```
My Name is [YOUR NAME].

My favorite color is [YOUR FAVORITE COLOR].
```

So for example, my file would look like:

```
My Name is Nick.

My favorite color is green.
```

As we can see here:

![screenshot](15.png)

After that have Partner A save the file and commit the change to the file's version history.

![screenshot](16.png)

After that, Partner A should also push their changes up to the repo.

![screenshot](17.png)

At this point Partner A's repo is all up to date. But Partner B is now no longer in sync. Partner B will need to fetch from the origin and pull down the new file and updates to the repository.

Let's do that now.

![screenshot](18.png)

![screenshot](19.png)

And now Partner B should see the file `demo.txt` in their local repo folder.

![screenshot](20.png)

Now, Partner B should open up the file and add in their name to line 5 and their favorite color to line 7.

![screenshot](21.png)

After that, Partner B should save, commit, and push their changes.

Then, after that Partner A should pull down Partner B's updates.

Now with the new updated file, Partner A should add in a new statement on line 9. Saying `But obviously the BEST color is purple.`.

![screenshot](22.png)

Then Partner A should save, commit, and push their changes. 

![screenshot](23.png)

Partner B will now need to pull down the changes. They should now see the new line.

![screenshot](24.png)

Partner B should now edit that line and change the BEST color to their favorite color. 

Partner B should save the file. Make a commit. (don't forget to leave nice descriptive commit messages - like Logan's example in the screenshot.)

Then push your changes up to the origin.

![screenshot](25.png)

Now.

We want to showcase a "merge-conflict" - aka - when we work with others, try to combine all our work together, but we edited the same line, so now we need to resolve the issue.

So, Partner A should open up their `demo.txt`.

They should also edit line 9 and change the "BEST" color to their favorite color.

![screenshot](26.png)

Partner A should save the file and make a commit.

![screenshot](27.png)

Partner A should then try to push. But We will now see a merge conflict! Oh no!

![screenshot](28.png)

![screenshot](29.png)

Partner A should now follow the prompt and perform a fetch.

![screenshot](30.png)

![screenshot](31.png)

![screenshot](32.png)

Now, let's resolve this merge conflict just like how we demonstrated in class.

As a reminder, the `<<<<<<<` shows where the conflict begins, the `=======` is the seperation between the two possible conflict points, and the `>>>>>>>>` is the end of the conflict.

![screenshot](33.png)

![screenshot](34.png)

After the conflict has been resolved. Don't forget to save the file. After you save, GitHub Desktop should recognize that you resolved the conflict.

![screenshot](35.png)

Now click `continue merge`.

We now need to commit the merge conflict resolution to the version control history of the file. Go ahead do that, then push your changes to the origin.

![screenshot](36.png)

At this point, Partner B can pull down the updates and your team can refresh GitHub.com

We should now see the final version of our exercise, where the conflict has been resolved, and we all now live in peace and harmony. :)

![screenshot](37.png)

![screenshot](38.png)

## Conclusion

At this point, your team has successfully recreated the demonstration from class. Time to celebrate this is a major skill addition. A lot of programmers (32.33% repeating of course) are too afraid of dealing with merge conflicts. 

![screenshot](home_alone.gif)

## Submitting

Don't forget to submit to the mycourses dropbox. See the assignment for submission guidelines.