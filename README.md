# qaylene's ToDo Application


## Summary
Assignment 2 for HMC CS 121, Fall 2017 <br>
Create a user account for this desktop ToDo Application to more easily manage your tasks. This application displays all your current and completed tasks in one page. 


## Minimum Viable Product (MVP)
Users have the option of creating new tasks, with each task consisting of a "Title," "Note," and "Completed" section which users can use to name their task, include some notes specific to the task, and assign a date completed, respectively. Tasks show up in a table on the home page where each task can be edited and deleted.

## Functionalities

### Home Page
Users can view all their current and completed tasks and also manage their tasks by editing or deleting selected tasks. 
<p align="center">
	<img src="https://user-images.githubusercontent.com/12602569/30793188-0b09d156-a175-11e7-8895-83f5301726a3.png" width="500" > 
</p>

### Signup
Users can enter their email and a password to register for an account.
<p align="center">
	<img src="https://user-images.githubusercontent.com/12602569/30793194-1083803c-a175-11e7-998e-cb5e5b4adad1.png" width="500" > 
</p>

### Login/Logout
Users can log in to their account.
<p align="center">
	<img src="https://user-images.githubusercontent.com/12602569/30793191-0c94a3fc-a175-11e7-9766-097e65041a7b.png" width="500" > 
</p> 

### New Task
Users can create a new task with a title, notes, and completed date. 
<p align="center">
	<img src="https://user-images.githubusercontent.com/12602569/30793192-0e984af0-a175-11e7-9730-e90428f46d11.png" width="500" > 
</p>

### Edit Task
Users can edit existing tasks. 
<p align="center">
	<img src="https://user-images.githubusercontent.com/12602569/30793184-08f1bf0a-a175-11e7-9de1-246b6ed2949f.png" width="500" > 
</p>

## Delete Task
Users can delete existing tasks. A prompt will appear to comfirm deleting the task.  


## Architecture
- Main Page: Users can view and manage all their tasks here. <br>
- Users: Users can manage their tasks through creating new ones, editing existing ones, or deleting certain tasks. <br>
- Tasks: Each task consists of a "Title," "Note," and "Completed" section where users can input the name of the task, notes about the task, and the completed date (format: dd/mm/yy). 


## Fixed Issues and their Solutions
1. Creating a new task created two tasks instead of one
 * Solution: Removed the "//= require jquery_ujs" as multiple jquerys can lead to duplications in actions (https://github.com/rails/jquery-ujs/issues/208)

## Known Bugs
1. Calendar does not show up for Completed date selection
2. Creating/Editing/Deleting new task reloads page to show all tasks rather than those specific to that user


## Resources:
- ToDo Application tutorial:
    * http://iridakos.com/2013/12/07/creating-a-simple-todo-part-1.html
    * http://iridakos.com/2013/12/17/creating-a-simple-todo-part-2.html
    * http://iridakos.com/2013/12/20/creating-a-simple-todo-part-3.html
- References used to solve issues:
   * https://github.com/rails/jquery-ujs/issues/208
