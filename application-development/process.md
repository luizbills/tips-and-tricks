## Understand the problem.
Know what “make it work” means.

## Begin at the beginning.
If the task is to identify what the current user is doing, the first step is probably to identify who the current user is.

## Do one thing (DOT)
Don’t try to squeeze all the app requirements into the first module you write. Chances are your finished app will consist of many modules. Keep each module small and focused, and concentrate on one module at a time.

- Do **one thing per line**.
- Do **one thing per function**. For example, if you need to use the value of a query parameter, you should dedicate a function to extracting the value of a query parameter from the URL rather than mix that logic with a function that uses the value.
- Use **one variable to represent only one thing**. 

## Start small and iterate.
Write a test. Make it pass. Refactor. Make it work. Make it right. Make it fast. One step at a time. Keep taking those steps until the job is done.
