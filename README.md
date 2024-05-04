# Git-and-Github
In this repo, I'll try to talk about Git and Github

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
