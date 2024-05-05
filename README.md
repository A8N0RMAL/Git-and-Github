![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/b687989b-5c6e-41f1-940c-e8855b0513fe)# Git-and-Github
In this repo, I'll try to talk about Git and Github
![git-vs-github](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/a1024356-895b-4b2d-9f30-6cb4781ec21e)

---
### What are we gonna learn through this course:
- Git and Github.
- Git basics.
- Branches.
- Merge.
- Working with remote repository.
- Some Useful plugins.
---
#### Git and Github
- What is Version Control?
1. A tool for managing changes related to code and files within a project.
2. It allows you to track all modifications along with their timestamps.
3. Additionally, it enables you to store a copy of files on your personal computer or on the tool, such as Git, used for version control application.

---

- What is Git?
- Git is one of the most popular types of version control systems used to apply version control to software.
1. Git is a distributed version control system (DVCS).
2. It enables multiple users to collaborate on projects.
3. Git tracks changes to files and manages different versions of code.
4. Linus Torvalds created Git in 2005 to manage the Linux kernel's development.
5. It has become widely used for managing source code of various software projects.
6. Git offers features like branching, merging, and distributed workflows.
7. These features make it powerful and flexible for small and large-scale development projects.

- There are many different programs used to implement version control, such as:
1. CVS.
2. SVN.
3. Perforce.
4. Bazaar.

---
##### Git vs. Github:
- What is the difference between Git vs. Github?
- Git : Version control, which manages changes related to code and files within the project, it manages code and file changes locally.
- Github : A cloud-based platform, allows for managing and organizing files (Git Repos) and facilitates sharing and editing projects from any device.
  
![image](https://github.com/A8N0RMAL/Gita-and-Github/assets/119806250/101ec355-de13-4f84-8398-0bbfe9cb0495)

---
- What is git init?
- The command git init is used to create a new Git repository.
- It's used for your current project or to start a repository when you need to create one.
- Git initializes a new project by creating a new folder in the current path.
- When you run git init, Git uses this folder to store all data, such as project history, version logs, and other information, named ".git".

- Let's take a look: Now the folder is empty.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/52aa5b57-2581-45b4-9811-934912cb458d)
- Open cmd in this folder and run the git init command.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/87c479bd-2620-4746-8024-b048b0bc34f6)
- Now we can see the .git folder that stores all data such as project history, version logs and other information about your projects.
- NOTE : if u cannot show the icon of .git folder just make sure to show hidden files.

---
- What is git add?
- The command git add is used to add the specified files to the staging area, which is the next commit.
- It allows you to specify the files to be included in the upcoming commit, followed by the filenames.
- Staged files are files that are ready to be committed to the repository you are working on. You will learn more about commit shortly.
- For now, we have a file named index.html. So we can add it to the Staging Environment:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/1f26f9d3-4214-4e0f-8820-0648d66377ed)
- Now the file is added successfully.
- The file should be Staged. Let's check the status:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/4f8cc4e3-99d9-4a54-b7c7-ee35e5793099)
- Now the file has been added to the Staging Environment.
- We can also stage more than one file at a time. using git add --all
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/6a2b05b5-0b55-4d54-9ea6-c25010d4fe4a)
- Now let's check the status using git status to ensure that all files are at the staging area.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/ea262217-0d79-43b7-abb0-925a400d2c4c)
- As we can see the files are added to the staging area successfully.
- Let's take some Examples:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/4451d889-0212-40cf-a5b8-c505ee76105e)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/c433741a-e703-4f61-9b6f-53bbfddb5db9)
---
- What is git commit?
- The command git commit is used to save the changes that have been added to your staging area, It applies them to your repository.
- A new git commit followed by a message can be used to create a description of the changes you've made. For example, git commit -m "added new files".
- With git commit, the changes you've made are permanently stored in your repository, allowing you to revert to them at any time to update your project or restore a previous version.
- When we commit, we should always include a message.
- By adding clear messages to each commit, it is easy for yourself (and others) to see what has changed and when.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/2ae89cd9-4cae-4cdd-8c33-e0598940d138)
- The commit command performs a commit, and the -m "message" adds a message.
##### Git Commit without Stage
- Sometimes, when you make small changes, using the staging environment seems like a waste of time. It is possible to commit changes directly, skipping the staging environment. The -a option will automatically stage every changed, already tracked file.
- Let's add a small update to index.html:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/68a3e370-b535-4b61-9111-e7f5fc823d81)
- And check the status of our repository. But this time, we will use the --short option to see the changes in a more compact way:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/24c18ffc-55f4-4fd1-bc1f-11760a106847)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/244d40c8-c5bc-4e88-82a9-a0295af3bc38)
- We see the file we expected is modified. So let's commit it directly:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/606dab5d-e0b6-4327-8ce9-249957a6a543)
- Warning: Skipping the Staging Environment is not generally recommended.
- Skipping the stage step can sometimes make you include unwanted changes.
- To view the history of commits for a repository, you can use the log command:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/ac4dba30-5fa0-4a51-a5c2-604692371723)
- Let's dig into some more examples of git commit:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/62fecfd6-0881-4391-adfd-971941f4ca8d)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/1669c364-9583-446a-8f6b-0e3f7b1976c1)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/4de7e43c-f715-4db6-8d97-c1e6201236b3)
---
- What is git log?
- "Git log" is a command used to display the Git commit history in a repository.
- It lists all commits in the current branch.
- This command displays information such as the commit hash, author, date, and commit message, for every commit in the repository.
- Git log can be used to understand the repository's history and analyze its evolution generally.
- Moreover, it can be used as a tool to locate and review errors.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/06206f5f-20ff-4182-a1f6-8b3347b01c95)
---
- What is .gitignore file?
- When sharing your code with others, there are often files or parts of your project, you do not want to share.
- Examples:
1. log files
2. temporary files
3. hidden files
4. personal files, etc.
- Git can specify which files or parts of your project should be ignored by Git using a .gitignore file.
- The '.gitignore' file is created within the project's working directory and contains a list of files and directories that should be ignored when tracking changes in the project using Git.
- When you create a new file or directory within the working directory, Git will include it when you initialize a repository.
- However, there may be files or directories that Git should not track changes for using unnecessary or unwanted files, such as configuration files or files containing sensitive or temporary information.
- The ".gitignore" file can be used to instruct Git to ignore these files, so they are not tracked within the history logs and versions.
#### Create .gitignore
- To create a .gitignore file, go to the root of your local Git, and create it:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/7fab6eb6-3ba7-4d27-baa6-60366c1fe009)
- Now open the file using a text editor.
- We are just going to add two simple rules:
- Ignore any files with the .log extension
- Ignore everything in any directory named temp
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/ba1dc849-b064-4868-a5c9-53dcc0ea073e)
- Now all .log files and anything in temp folders will be ignored by Git.
- Note: In this case, we use a single .gitignore which applies to the entire repository.
- It is also possible to have additional .gitignore files in subdirectories. These only apply to files or folders within that directory.
#### Rules for .gitignore
- Here are the general rules for matching patterns in .gitignore files:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/8e53ff34-5ae4-4bd7-84b1-c08f2e45fd21)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/b31fbcf5-6460-461b-b810-cd1ba3f18097)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/a3f38153-8258-4cba-9adf-d9bc5eafa2c7)
#### Local and Personal Git Ignore Rules
- It is also possible to ignore files or folders but not show it in the distributed .gitignore file.
- These kinds of ignores are specified in the .git/info/exclude file. It works the same way as .gitignore but are not shown to anyone else.
- Here are some examples of .gitignore:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/3899c127-8e35-48f9-bb2b-d476e931d988)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/9dd1fb0c-9dfd-44fe-8abd-a26f36685de8)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/d182d2a8-f188-469d-8c47-145a09ad1374)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/c0a0eda5-6c70-44aa-b0af-1c01be2f2ab8)
---
- What is Branch?
- Branches allow you to develop different paths for changes in Git.
- With a new branch, you can develop or make changes to your own branch.
- When creating a Git branch repository, changes can be made without affecting other parts that other teams are working on in the same project. In other words, you will take a copy of the project, make modifications to it, and the main project will not be affected by any changes you make.
- After ensuring that what you have added or modified is correct, you can add it to the main project.
##### Let's take a look more deeper:
- In Git, a branch is a new/separate version of the main repository.
- Let's say you have a large project, and you need to update the design on it.
- How would that work without and with Git:
#### Without Git:
- Make copies of all the relevant files to avoid impacting the live version
- Start working with the design and find that code depend on code in other files, that also need to be changed!
- Make copies of the dependant files as well. Making sure that every file dependency references the correct file name
- EMERGENCY! There is an unrelated error somewhere else in the project that needs to be fixed ASAP!
- Save all your files, making a note of the names of the copies you were working on
- Work on the unrelated error and update the code to fix it
- Go back to the design, and finish the work there
- Copy the code or rename the files, so the updated design is on the live version
- (2 weeks later, you realize that the unrelated error was not fixed in the new design version because you copied the files before the fix)
#### With Git:
- With a new branch called new-design, edit the code directly without impacting the main branch
- EMERGENCY! There is an unrelated error somewhere else in the project that needs to be fixed ASAP!
- Create a new branch from the main project called small-error-fix
- Fix the unrelated error and merge the small-error-fix branch with the main branch
- You go back to the new-design branch, and finish the work there
- Merge the new-design branch with main (getting alerted to the small error fix that you were missing)

- Branches allow you to work on different parts of a project without impacting the main branch.
- When the work is complete, a branch can be merged with the main project.
- You can even switch between branches and work on different projects without them interfering with each other.
- Branching in Git is very lightweight and fast!
##### New Git Branch
- Let add some new features to our index.html page.
- We are working in our local repository, and we do not want to disturb or possibly wreck the main project.
- So we create a new branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/a13738e5-cf00-4e83-bd57-7395178eb713)
- Now we created a new branch called "hello-world-images"
- Let's confirm that we have created a new branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/fbb6660e-ee31-47bd-828f-19b8a22e9af6)
- We can see the new branch with the name "hello-world-images", but the * beside master specifies that we are currently on that branch.
- checkout is the command used to check out a branch. Moving us from the current branch, to the one specified at the end of the command:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/096d4323-15f2-4098-bfef-b9beab7fa5da)
- Now we have moved our current workspace from the master branch, to the new branch
- Open your favourite editor and make some changes.
- For this example, we added an image (img_hello_world.jpg) to the working folder and a line of code in the index.html file:
- So let's go through what happens here:
- There are changes to our index.html, but the file is not staged for commit
- img_hello_world.jpg is not tracked
- So we need to add both files to the Staging Environment for this branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/ae6a21b6-1334-4a7d-95de-d1ba6fe2716e)
- Using --all instead of individual filenames will Stage all changed (new, modified, and deleted) files.
- Check the status of the branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/29a47b07-16a9-4932-a1f3-3bf99f1a7c6c)
- We are happy with our changes. So we will commit them to the branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/df3d4643-21a9-49d2-b30d-83b4db4e7cdb)
- Now we have a new branch, that is different from the master branch.
- Note: Using the -b option on checkout will create a new branch, and move to it, if it does not exist.
#### Switching Between Branches
- Now let's see just how quick and easy it is to work with different branches, and how well it works.
- We are currently on the branch hello-world-images. We added an image to this branch, so let's list the files in the current directory:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/ba55536d-17f4-4a62-8881-40f29f953d0d)
- We can see the new file img_hello_world.jpg, and if we open the html file, we can see the code has been altered. All is as it should be.
- Now, let's see what happens when we change branch to master.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/18bb08a9-6aaa-4fb1-b08a-a5be44878f85)
- The new image is not a part of this branch. List the files in the current directory again:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/2dda1236-104f-4fbb-a632-5227c7593934)
- img_hello_world.jpg is no longer there! And if we open the html file, we can see the code reverted to what it was before the alteration.
- See how easy it is to work with branches? And how this allows you to work on different things?
#### Emergency Branch
- Now imagine that we are not yet done with hello-world-images, but we need to fix an error on master.
- I don't want to mess with master directly, and I do not want to mess with hello-world-images, since it is not done yet.
- So we create a new branch to deal with the emergency:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/58d33566-363d-4b3f-9233-cab820415870)
- Now we have created a new branch from master, and changed to it. We can safely fix the error without disturbing the other branches.
- Let's fix our imaginary error:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/e7d454e1-9a66-43d3-a86f-5e81b06e4fe8)
- We have made changes in this file, and we need to get those changes to the master branch.
- Check the status:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/1439a1cc-f297-4561-924f-3d517a538096)
- stage the file, and commit:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/c368c9e2-7e2a-4077-8812-81abf908f9e1)
- Now we have a fix ready for master, and we need to merge the two branches.
- Here are some examples of Git branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/f7a7765c-76c9-495e-b8fe-b16afcb84361)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/7b0a7385-d3c3-49f5-9dae-84eeab8c6a93)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/dace61f6-0a4d-47ec-b887-1c95ea934ca3)
---
- What is Branch?
- Branches allow you to develop different paths for changes in Git.
- With a new branch, you can develop or make changes to your own branch.
- When creating a Git branch repository, changes can be made without affecting other parts that other teams are working on in the same project. In other words, you will take a copy of the project, make modifications to it, and the main project will not be affected by any changes you make.
- After ensuring that what you have added or modified is correct, you can add it to the main project.
##### Let's take a look more deeper:
- In Git, a branch is a new/separate version of the main repository.
- Let's say you have a large project, and you need to update the design on it.
- How would that work without and with Git:
#### Without Git:
- Make copies of all the relevant files to avoid impacting the live version
- Start working with the design and find that code depend on code in other files, that also need to be changed!
- Make copies of the dependant files as well. Making sure that every file dependency references the correct file name
- EMERGENCY! There is an unrelated error somewhere else in the project that needs to be fixed ASAP!
- Save all your files, making a note of the names of the copies you were working on
- Work on the unrelated error and update the code to fix it
- Go back to the design, and finish the work there
- Copy the code or rename the files, so the updated design is on the live version
- (2 weeks later, you realize that the unrelated error was not fixed in the new design version because you copied the files before the fix)
#### With Git:
- With a new branch called new-design, edit the code directly without impacting the main branch
- EMERGENCY! There is an unrelated error somewhere else in the project that needs to be fixed ASAP!
- Create a new branch from the main project called small-error-fix
- Fix the unrelated error and merge the small-error-fix branch with the main branch
- You go back to the new-design branch, and finish the work there
- Merge the new-design branch with main (getting alerted to the small error fix that you were missing)

- Branches allow you to work on different parts of a project without impacting the main branch.
- When the work is complete, a branch can be merged with the main project.
- You can even switch between branches and work on different projects without them interfering with each other.
- Branching in Git is very lightweight and fast!
##### New Git Branch
- Let add some new features to our index.html page.
- We are working in our local repository, and we do not want to disturb or possibly wreck the main project.
- So we create a new branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/a13738e5-cf00-4e83-bd57-7395178eb713)
- Now we created a new branch called "hello-world-images"
- Let's confirm that we have created a new branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/fbb6660e-ee31-47bd-828f-19b8a22e9af6)
- We can see the new branch with the name "hello-world-images", but the * beside master specifies that we are currently on that branch.
- checkout is the command used to check out a branch. Moving us from the current branch, to the one specified at the end of the command:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/096d4323-15f2-4098-bfef-b9beab7fa5da)
- Now we have moved our current workspace from the master branch, to the new branch
- Open your favourite editor and make some changes.
- For this example, we added an image (img_hello_world.jpg) to the working folder and a line of code in the index.html file:
- So let's go through what happens here:
- There are changes to our index.html, but the file is not staged for commit
- img_hello_world.jpg is not tracked
- So we need to add both files to the Staging Environment for this branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/ae6a21b6-1334-4a7d-95de-d1ba6fe2716e)
- Using --all instead of individual filenames will Stage all changed (new, modified, and deleted) files.
- Check the status of the branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/29a47b07-16a9-4932-a1f3-3bf99f1a7c6c)
- We are happy with our changes. So we will commit them to the branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/df3d4643-21a9-49d2-b30d-83b4db4e7cdb)
- Now we have a new branch, that is different from the master branch.
- Note: Using the -b option on checkout will create a new branch, and move to it, if it does not exist.
#### Switching Between Branches
- Now let's see just how quick and easy it is to work with different branches, and how well it works.
- We are currently on the branch hello-world-images. We added an image to this branch, so let's list the files in the current directory:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/ba55536d-17f4-4a62-8881-40f29f953d0d)
- We can see the new file img_hello_world.jpg, and if we open the html file, we can see the code has been altered. All is as it should be.
- Now, let's see what happens when we change branch to master.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/18bb08a9-6aaa-4fb1-b08a-a5be44878f85)
- The new image is not a part of this branch. List the files in the current directory again:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/2dda1236-104f-4fbb-a632-5227c7593934)
- img_hello_world.jpg is no longer there! And if we open the html file, we can see the code reverted to what it was before the alteration.
- See how easy it is to work with branches? And how this allows you to work on different things?
#### Emergency Branch
- Now imagine that we are not yet done with hello-world-images, but we need to fix an error on master.
- I don't want to mess with master directly, and I do not want to mess with hello-world-images, since it is not done yet.
- So we create a new branch to deal with the emergency:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/58d33566-363d-4b3f-9233-cab820415870)
- Now we have created a new branch from master, and changed to it. We can safely fix the error without disturbing the other branches.
- Let's fix our imaginary error:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/e7d454e1-9a66-43d3-a86f-5e81b06e4fe8)
- We have made changes in this file, and we need to get those changes to the master branch.
- Check the status:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/1439a1cc-f297-4561-924f-3d517a538096)
- stage the file, and commit:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/c368c9e2-7e2a-4077-8812-81abf908f9e1)
- Now we have a fix ready for master, and we need to merge the two branches.
- Here are some examples of Git branch:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/f7a7765c-76c9-495e-b8fe-b16afcb84361)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/7b0a7385-d3c3-49f5-9dae-84eeab8c6a93)
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/dace61f6-0a4d-47ec-b887-1c95ea934ca3)
---
#### Let's take a look at Branch Visualization:
- Shall we get our hand dirty ?
- Visit this site -> https://learngitbranching.js.org/
- This is our site before making anything:
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/0fbde0f5-cc2a-4f73-8fc7-d2de38a3b92c)
- Let's add some commits for main
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/4d11a08a-b772-48e4-9921-3b4bcf84ad8d)
- make a new branch called file-edit
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/7afbf903-0c7d-4b19-baf7-fbd3810f3a9e)
- Now u cannot make changes on file-edit, so we can use the command git checkout to move to file-edit branch and make wahtever we want.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/5dd6841e-e772-4c0b-8600-5197245a4439)
- Now u can see the asterik is on the branck called file-edit
- add some commits for this branch
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/bead15a4-7ec0-4a22-9a55-d800556bf943)
- Now u can see that the changes don't affect the main project, Only the file-edit branch can affected by them.
- If u wanna go back to the main, just use git checkout place(main) in this case.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/889b5170-3a92-479f-b5a3-d856be96ca42)
- Now we're on the main, let's make a new branch called file-down and move to it using git checkout file-down command and make some commits, here is the result.
![image](https://github.com/A8N0RMAL/Git-and-Github/assets/119806250/e362cce5-711a-480f-9d91-e28d370f6a44)
- As we can see, Changes don't affect the main project, Each branch on its own.
---
