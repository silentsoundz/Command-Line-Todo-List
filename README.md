# Command-Line-Todo-List

## Description

Write a command line script called `tasks` that allows the user to manage a list
of tasks from the terminal.

Your `tasks` command should support the following sub-commands:

| command  | description                                            | example usage                       |
|----------|--------------------------------------------------------|-------------------------------------|
| add      | adds the specified task                                | ./tasks add Finish reading Flatland |
| list     | lists the incomplete tasks                             | ./tasks list                        |
| complete | marks the task with `id` equal to `<task-id>` complete | ./tasks complete `<task-id>`        |
| delete   | deleted the specified task                             | ./tasks delete `<task-id>`          |


In this 1st version the data for your tasks should be saved to a file called
`tasks.json`.


## Specs

- [ ] Your command should be called `tasks`
- [ ] The `tasks` command file should have a shebang pointing to `node`
- [ ] The `tasks` command file should have execute permissions
- [ ] Tasks are persisted to a `json` file using `fs.readFileSync` and `fs.writeFileSync`
- [ ] The `list` command is implemented in `./commands/list.js`
- [ ] The `add` command is implemented in `./commands/add.js`
- [ ] The `complete` command is implemented in `./commands/complete.js`
- [ ] The `delete` command is implemented in `./commands/delete.js`
- [ ] Add tests using Mocha and Chai for all functions
- [ ] User receives an error message if they enter an invalid command
- [ ] Your program should create the `tasks.json` if the file doesn't exist
- [ ] `tasks.json` is ignored and not checked into your Git repository
