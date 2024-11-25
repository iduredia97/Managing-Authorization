# Managing-Authorization
## Objective
Review and edit user, group and other permissions on project files using Linux commands in a Bash shell.
## Necessary Permission Changes
* Remove write permissions for other on file **project_k.txt**.
* Remove read permissions for group on file **project_m.txt**.
* Remove write permissions from user and group on file **.project_x.txt**.
* Add read permissions to group on file **.project_x.txt**.
* Remove executable permissions from group on directory **/home/researcher2/projects/drafts**.
## Steps taken
* Navigate to projects directory using ```cd projects```.
* List non-hidden files and directories using ```ls```.
* Reviewed permissions for non-hidden files and directories found in the **/home/researcher2/projects** directory using ```ls- l```.

![screenshot1](https://github.com/iduredia97/Managing-Authorization/blob/main/1.png)

* Reviewed permissions for hidden files and directories found in the **/home/researcher2/projects** directory using ```ls -la```.

![screenshot2](https://github.com/iduredia97/Managing-Authorization/blob/main/2.png)

* Removed write permissions from other on file **project_k.txt** using ```chmod o-w project_k.txt```.
* Verified updated permissions on file **project_k.txt** using ```ls -l project_k.txt```.

![screenshot3](https://github.com/iduredia97/Managing-Authorization/blob/main/3.png)

* Removed read permissions from group on file **project_m.txt** using ```chmod g-r project_m.txt```.
* Verified updated permissions on file **project_k.txt** using ```ls -l project_m.txt```.

![screenshot4](https://github.com/iduredia97/Managing-Authorization/blob/main/4.png)

* Removed write permissions from user and group & added read permissions to group on file **.project_x.txt** using ```chmod u-w,g-w,g+r .project_x.txt```.
* Verified updated permissions on file **.project_x.txt** using ```ls -la .project_x.txt```.

![screenshot5](https://github.com/iduredia97/Managing-Authorization/blob/main/5.png)

* Reviewed permissions of directory **/home/researcher2/projects/drafts** using ```ls -ld drafts```.
* Removed executable permissions from group on directory **/home/researcher2/projects/drafts** using ```chmod g-x drafts```.
* Verified updated permissions of directory **/home/researcher2/projects/drafts** using ```ls -ld drafts```.

![screenshot6](https://github.com/iduredia97/Managing-Authorization/blob/main/6.png)
