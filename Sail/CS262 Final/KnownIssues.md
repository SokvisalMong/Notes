## Port 3306 is in-use

Cause: MySQL starts on boot

This happens to my team members who use windows.

Solution: Open Task Manager > Services > MySQL > Stop Task

Not the most elegant but ehh.

## Permission Issues

If you are having permission issues, make sure that the user you installed the laravel sail app with

and the current user is the same one.

For example:

```
dev@VizzyPC:~/
```

was used to install Laravel.

Then make sure the stick with that.

Especially becareful with screen.