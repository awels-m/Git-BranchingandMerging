# Git-BranchingandMerging
here i will be submitting my project on Git branching and merging

# OBJECTIVE OF THE PROJECT 
Here i will be learning how to merge and branch changes. I am alos going to create a pull request and then merge the pull request into the main branch. A pull request is a feauture used in GitHub that allows you notify team members about changes you pushed to a branch in a repository. Essentially, its a request to review and pull in your contribution to the main project.

# HOW TO CREATE A PULL REQUEST
After Tom and Jerry have pushed their work to their respective branches, the next thing to do is to pull the request for his changes. 
A pull request (PR) is a way of notifying others that you’ve made changes to a codebase and are requesting those changes be reviewed and merged into the main branch. It allows team members to discuss the proposed modifications, review the code for quality, suggest improvements, and ensure the new code integrates well with the existing codebase. Creating a pull request is a standard best practice in collaborative software development to maintain code integrity and facilitate version control.


## NAVIGATE TO YOUR GITHUB REPOSITORY. 
I opened my web browser and went to my github page for the repository. the image below depicts this 
![1img](./1img.png)

## SWITCH THE BRANCH TO MAIN
The image below depicts this.
![2img](./2img.png)
![4img](./4img.png)

How to Switch Branches to main on GitHub Website
	1.	Go to your repository on GitHub.
	2.	At the top-left of the repo file list, you’ll see a branch dropdown. It usually shows your current branch name (e.g., feature-branch, dev, etc).
	3.	Click on that branch dropdown.
	4.	In the search box that appears, type main.
	5.	Click on main from the list.

You’re now viewing the main branch of your repository.

## CREATE NEW PULL REQUEST AND REVIEW TOMS CHANGES
The image below depicts this 
![3img](./3img.png)
![5img](./5img.png)
![6img](./6img.png)
![16img](./16img.png)
![18img](./18img.png)
These shows that the pull request for Tom was successful and its now time to merge the changes. the image below depicts this.

## MERGE THE CHANGES OF TOM
the image below depicts this 
![7img](./7img.png)
![8img](./8img.png)

## UPDATE JERRYS BRANCH
### SWITCH TO JERRYS BRANCH
This is done by running this command - git checkout add-contact-info
The image below depicts this
![9img](./9img.png)
![10img](./10img.png)

## PULL THE LATEST CHANGES FROM THE MAIN BRANCH
this is done by running this command - git pull origin main
the image below depicts this
![11img](./11img.png)
![12img](./12img.png)

## FINALIZING JERRYS CONTRIBUTION
The first to do is to push the updated branch to github
this is done by running this command "git push origin add-contact-info"
the image below depicts this
![14img](./14img.png)

## CREATE A PULL REQUEST
A pull request is a way to propose changes you’ve made in a separate branch be added to the main project. It allows others to review your work, suggest improvements, and approve it before it’s merged. This helps ensure code quality, avoid conflicts, and keep the project organized—especially when working in a team.

The image below depicts this
![15img](./15img.png)
![17img](./17img.png)
![19img](./19img.png)
![20img](./20img.png)
![21img](./21img.png)

the images above shows that the pull request was done successfully and I can proceed to merge the changes. 

## MERGE JERRY'S PULL REQUEST. 
The image below depicts this 
after iy has been reviewd, i can now successfully merge as seen in the image below. 
![22img](./22img.png)
![23img](./23img.png)

The image above shows that Jerrys Work from his branch was successfully merged. This brings me to the end of this project. 

# CONCLUSION

This project has given me practical experience in working with Git branching and merging, both through the GitHub interface and via the Linux terminal. I created and managed separate branches for two users, Tom and Jerry, each making changes to the same file. I successfully created and merged pull requests for both contributors—one using the GitHub website and the other through terminal commands. I encountered a real challenge during Jerry’s merge and resolved it by updating my Git configuration. This not only helped me understand common Git errors but also made me more confident using Git professionally. Overall, the project solidified my understanding of collaborative version control and gave me a strong foundation for future teamwork in software development.


## Project Topic: GIT BRANCHING AND MERGING

### Project Overview

This project focused on practicing how to work with multiple branches in Git and how to merge changes using pull requests, both via the GitHub website and the Linux terminal. The scenario involved two contributors, Tom and Jerry, who each had their own separate branch — Tom’s branch was named update-navigation, while Jerry’s branch was named add-contact-info.

Both contributors made changes to the same file, index.html, but on their respective branches. The objective of this project was to merge their separate changes into the main branch without conflicts, following the proper Git workflow.

### Step-by-Step Workflow and Explanation

#### Step 1: Navigating to the Repository (Tom’s Changes)

The first thing I did was to go to my GitHub repository on the web. From there, I switched from the default main branch to Tom’s branch, update-navigation. I needed to do this so I could initiate a pull request from Tom’s branch into main.

#### Reason: You always create a pull request from the feature branch (in this case, Tom’s branch) into the base branch, which is usually main.

#### Step 2: Creating a Pull Request for Tom

Once on the update-navigation branch, I clicked on “Compare & pull request”. GitHub automatically detected that the update-navigation branch had new changes that could be merged into main. I reviewed the changes, ensured there were no conflicts, and then clicked “Merge pull request” to successfully integrate Tom’s changes into the main branch.

#### Reason: Pull requests on GitHub allow for change review, team collaboration, and safe merging. It’s a good habit even when working solo.

#### Step 3: Switching to Terminal for Jerry’s Changes

Unlike Tom’s merge which was done entirely on GitHub, I decided to work with Jerry’s changes on my Linux terminal. This was to practice how Git commands work locally.

First, I used the command:
git checkout add-contact-info
This switched my working directory to Jerry’s branch.

#### Reason: Before updating or pushing changes on a branch, you must switch to that branch using git checkout.

#### Step 4: Pulling the Latest Changes from main

I wanted to ensure that Jerry’s branch was up-to-date with whatever was currently in the main branch — especially since Tom’s work had already been merged into main. To do this, I ran:
git pull origin main

But here, I faced a challenge — Git threw an error because of my local Git configuration.

#### Challenge Encountered

Git gave a warning about diverging branches and asked whether to merge or rebase. I resolved this by running:
git config pull.rebase false

#### Reason: This command tells Git to merge instead of trying to rebase during a pull, making it easier for beginners and less prone to confusion.

After setting that, I successfully pulled the latest changes from main into Jerry’s branch.

##### Step 5: Pushing Jerry’s Updated Branch

Now that Jerry’s branch had the latest changes from main, I pushed it back to GitHub with:
git push origin add-contact-info

#### Reason: After pulling updates and resolving any changes locally, you push the updated branch so that you can open a pull request on GitHub.

#### Step 6: Creating Pull Request for Jerry

I went back to GitHub, and this time GitHub showed the option to “compare & pull request” for add-contact-info. I clicked it, reviewed the file changes, and then clicked “Merge pull request” to successfully merge Jerry’s branch into main.

#### Result: Now, both Tom’s and Jerry’s changes had been safely and cleanly merged into the project.

## What I Learned
	•	How to switch between branches both on GitHub and in the terminal
	•	How to create and merge pull requests on GitHub
	•	How to use Git commands like checkout, pull, and push
	•	How to resolve pull-related conflicts using Git configuration
	•	The importance of updating feature branches with the latest changes from main before merging

### Feedback and Reflections

The Darey.io step-by-step guide was a big help in walking me through the basics of Git branching and pull requests. However, I didn’t stop there. I went further to explore:
	•	How Git handles merge conflicts behind the scenes
	•	How to use git rebase vs git merge
	•	What happens if multiple people edit the same lines of code

This research deepened my understanding of collaborative workflows and why Git is such a powerful tool in software development.

Also, I encountered a real challenge when Git refused to pull changes due to a configuration issue. Solving that by using git config pull.rebase false helped me understand how Git behaves when syncing branches — something I wouldn’t have learned if everything had gone smoothly.

## Conclusion

This project taught me how to properly handle real-world version control scenarios. I learned how to work with multiple branches, sync with the main branch, and merge contributions from different collaborators. I also now understand both the GitHub UI workflow and the terminal-based workflow, which gives me confidence to handle projects in any environment.

Mastering Git branching and merging is foundational for collaborative development, and I feel much more equipped to contribute to team projects going forward.