## DecentralizedTo-DoList
A simple Solidity smart contract for managing personal task lists on the Ethereum blockchain. This decentralized to-do list allows each user to securely create, update, and delete their own tasks.

# 🔐 Features


Each user can create, update, view, and soft-delete their own tasks.
Tasks are fully isolated per user address using mappings.
Task properties include:

taskID: Unique per user
title: Custom string title
status: One of Todo, InProgress, Blocked, or Done
createdAt: Timestamp of task creation
completedAt: Timestamp when marked as Done
isDeleted: Boolean flag for soft deletion

# ⚙️ Functionality


createTask(title): Add a new task with status set to Todo.
updateTask(taskID, status): Update a task’s status and mark the time of completion if done.
deleteTask(taskID): Soft-delete a task so it no longer appears in listings.
getMyTaskCount(): Returns the number of your active (non-deleted and non-completed) tasks.
getAllTasks(): Fetches all your tasks that haven’t been deleted.

# 🧱 Tech Stack


Language: Solidity v0.8.20
License: GPL-3.0
Designed for deployment on any EVM-compatible blockchain


