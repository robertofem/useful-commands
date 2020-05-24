Useful Commands
===============

Commonly used commands you look for in Stack Overflow.

Git
---

#### Fix file permissions

Fix the permissions of files in git repositories. Sometimes when you copy the folder of a git repository the permissions change, and then git interprets all files have suffered changes, when doing *git status*. You can revert those changes and leave the files that truly changed using this command:

```
git diff -p -R --no-ext-diff --no-color | grep -E "^(diff|(old|new) mode)" --color=never  | git apply
```

Devices
-------

#### Connect EasySMX ESM-9101 controller to Ubuntu

Install XBox driver:

```
sudo apt-get install xboxdrv
```

Connect the controller receiver to the PC and run:

```
sudo xboxdrv --device-by-id 2f24:0091 --type xbox360 --device-name 'EasySMX ESM-9101' --silent
```


