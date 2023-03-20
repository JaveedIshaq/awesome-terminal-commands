# awesome-terminal-commands
This repository is a reference for terminal commands and their usage. It includes commonly used commands with brief explanations for easy reference. It is designed to help users quickly access the commands they need, improve their command line proficiency, and streamline their workflow.

## ` ps ax | grep httpd`

The command ps ax | grep httpd is a Unix/Linux command that lists all running processes on the system and searches for any process whose name matches the keyword "httpd".

- ps stands for "process status" and is used to display information about running processes.
- ax is an option that tells "ps" to list all running processes from all users, rather than just the processes of the current user.
- | is a pipe operator that takes the output of the ps command and sends it as input to the next command.
- grep is a command that searches for a specific pattern in a text file or output.
httpd is the pattern being searched for in this case.

The overall command `ps ax | grep httpd` lists all running processes and searches for any process whose name contains "httpd". This is often used to check whether the Apache web server is currently running on a Unix/Linux system. If there is a running process with the name "httpd", it will be listed in the output along with its process ID (PID) and other information. If there is no running process with the name "httpd", the output will only show the "grep httpd" process itself.

## `brew services list`

`brew services list` is a command in the Homebrew package manager for macOS and Linux that lists all services managed by Homebrew on your system along with their current status. This command is especially useful for managing services that you have installed using Homebrew.

When you run the `brew services list` command, it displays a table with four columns:

- `Name`: The name of the service.
- `Status`: The current status of the service, which can be one of the following:
- `started`: The service is currently running.
- `stopped`: The service is not running.
- `error`: The service encountered an error when starting or stopping.
- `unknown`: The status of the service could not be determined.
- `none`: The service is installed but not currently being managed by Homebrew.
- `User`: The user account under which the service is running.
- `File`: The launch agent file that Homebrew uses to manage the service.

You can use the `brew services` command to manage the status of a service, start, stop or restart a service. This command is useful for managing and troubleshooting services installed with Homebrew.

Overall, brew services list is a convenient command that allows you to quickly see the status of all the services managed by Homebrew, making it easier to manage and troubleshoot services on your system.

Here are some examples of using the brew services command:

**Starting a service:**

`brew services start mysql`

This will start the mysql service, which may have been installed with Homebrew.

**Stopping a service:**

`brew services stop postgresql`

This will stop the postgresql service, which may have been installed with Homebrew.

**Restarting a service:**

`brew services restart apache2`

This will restart the apache2 service, which may have been installed with Homebrew.

**Viewing the status of a service:**

`brew services list`

This will list all services managed by Homebrew on your system along with their current status.

**Disabling a service from starting at login:**

`brew services stop mongodb`
`brew services cleanup mongodb`

This will stop the mongodb service and remove the launch agent file that Homebrew uses to manage the service, effectively disabling it from starting at login.

These are just a few examples of how to use the brew services command to manage and troubleshoot services installed with Homebrew.
