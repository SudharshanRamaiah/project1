Cross platform shell executor.

Using Jenkins built-in "Execute Windows batch command" you can run commands using the windows shell.

Using Jenkins built-in "Execute shell" you can run commands using unix shell.

If you need to run a job cross platform you cannot use the two standard executors provided by Jenkins. You need a "build step" that can be executed both in Windows and in Unix.

This plugin does exactly this: it takes a command, as the two standard build steps do, and executes it calling the correct shell depending on the operating system running on the current job executor.