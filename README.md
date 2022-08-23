# Kottans-frontend
---

#  Stage 0. Self-Study 

 - [x] **Git Basics**
 - [x] **Linux CLI and Networking**
 - [ ] **VCS (hello gitty), GitHub and Collaboration
 - [ ] **Intro to HTML & CSS
 - [ ] **Responsive Web Design
 - [ ] **HTML & CSS Practice
 - [ ] **JavaScript Basics
 - [ ] **Document Object Model - practice
 - [ ] **Building a Tiny JS World (pre-OOP) - practice
 - [ ] **Object oriented JS - practice
 - [ ] **OOP exercise - practice
 - [ ] **Offline Web Applications - optional
 - [ ] **Memory pair game — real project!
 - [ ] **Website Performance Optimization - optional
 - [ ] **Friends App - real project!

---
<h2 align="center">3)VCS (hello gitty), GitHub and Collaboration </h2> 

<details><summary><b>НЕДЕЛЯ 3-4 </b></summary>


![3](https://user-images.githubusercontent.com/65223481/186099852-a687c8c6-4dec-49c9-95fd-b5d3ab9d6016.png)


![4](https://user-images.githubusercontent.com/65223481/186099865-19f869d1-aecc-4562-82af-e6d059518cbd.png)

</details>


<hr/>
<h2 align="center">2) Linux CLI, and HTTP</h2> 

###  task_linux_cli

<details><summary> Quiz 1</summary>
  


![linux1](https://user-images.githubusercontent.com/65223481/184857947-66409b98-b1cb-457d-ad7e-2ca0098c771d.png)</details>
<details><summary> Quiz 2</summary>
  
![linux_2](https://user-images.githubusercontent.com/65223481/184943075-d3b2dd13-d4bc-4fbd-8a2a-03ebd42660af.png)</details>

<details><summary> Quiz 3</summary>
  
![linux3](https://user-images.githubusercontent.com/65223481/186087243-a6e7c107-b1fb-4b9d-9fce-6329f5f5c4be.png)


</details>
<details><summary> Quiz 4</summary>
  
![linux4](https://user-images.githubusercontent.com/65223481/186096113-377da8db-e62b-40b0-8492-4c528037bbca.png)



</details>


<hr/>
<h2 align="center">1) Git та GitHub</h2> 



 <details><summary>
 <b>НЕДЕЛЯ 1-2 </b></summary>

![n1](https://user-images.githubusercontent.com/65223481/182912787-c87eff3f-0ed6-4681-a8b7-aa87626b4309.png)

![n2](https://user-images.githubusercontent.com/65223481/182914206-2b5512e5-7d12-4ac8-b4c7-745cb56abac6.png)</details>



  <details><summary> <b> learngitbranching.js.org </b></summary>

![git](https://user-images.githubusercontent.com/65223481/184858362-2c894433-7643-4733-a1f4-9ac03a8bc0ea.png)

![git1](https://user-images.githubusercontent.com/65223481/184858837-e7c026c3-1101-47f3-8056-4fd3d20225e1.png)</details>


<details><summary> <b> Конспект </b></summary>
	
## Configuring you Git 

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git config --global user.name "Username" | Sets the name you want attached to your commit transactions |          
| $ git config --global user.email "Email" | Sets the email you want attached to your commit transactions |             
| $ git config --global color.ui auto | Colorization of command line output |                                 

	
 ## Creating Repository

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git init | Turn an existing directory into a git repository |          
| $ git clone [url] | Clone a repository that already exists on GitHub |             


 ## Operations on Files

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git add <filename> | Adds a file to Staging area |          
| $ git add * | Adds all files to Staging area | 
| $ git commit -a | Stages files automatically |
| $ git log -p | Produces patch text |
| $ git show | Shows various objects |
| $ git diff | Can show the differences in various commits |
| $ git diff --staged | Show all staged files compared to the named commit |
| $ git add -p | Allows a user to interactively review patches to add to the current commit |
| $ git mv | Moves a file |
| $ git rm | Removes a file |
	

## Reverting Changes 

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git reset | Resets the repo, throwing away some changes |          
| $ git commit --amend |  Make changes to commits |             
| $ git revert  | New commit which effectively rolls back a previous commit |


 ## Branches

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git branch | Used to manage branches |          
| $ git branch <name> | Creates the branch | 
| $ git branch -d <name> | Deletes the branch |
| $ git branch -D <name> | Forcibly deletes the branch |
| $ git checkout <branch> | Switches to a branch |
| $ git checkout -b <branch> | Creates a new branch and switches to it |
| $ git merge <branch> | Merge joins branches together |
| $ git merge --abort | abort the merge action (In case of merge conflict) |
| $ git log --graph --oneline | This shows a summarized view of the commit history for a repo |
	

## Interaction with Remote Repository

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git push | Git push is used to push commits from your local repo to a remote repo |          
| $ git pull | Git pull is used to fetch the newest updates from a remote repository |  


 ## Remotes

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git remote | Lists remote repos |          
| $ git remote -v | List remote repos verbosely | 
| $ git remote show <name> | Describes a single remote repo |
| $ git remote update | Fetches the most up-to-date objects |
| $ git fetch | Downloads specific objects |
| $ git branch -r | Lists remote branches; can be combined with other branch arguments to manage remote branches |
	
	 	

</details>
