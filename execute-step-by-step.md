$ARGUMENTS

Make sure task file is committed into git.

1. Do the next pending step in the task file.
2. After successfully completing a step
    2.1. update the task file to indicate progress
    2.2. git commit only the relevant files (do not bluntly git add everything) with conventional commit message style (specifying it is phase n/m of this task)
3. Loop back to (1) unless there are no more pending steps in the task file.

When we're all done, commit only the relevant files (do not bluntly git add everything) with conventional commit message style and let me know the current git status after that.
