# GitYoink
A git alias for force pulling.

Ever wished for a ``yoink`` command in git? Now you have it !
Simply type:
```
git yoink
```

To force pull from a repository.

### Setup Guide

Run the following command to define the ``yoink`` command as a force pull (discarding any local changes and resetting to the remote state)
```
git config --global alias.yoink '!git fetch origin && git reset --hard origin/$(git rev-parse --abbrev-ref HEAD)'
```

### Definition

From dictionary.com:

**Yoink** (verb)
1. to grab, pull, or take, especially abruptly or vigorously

E.i. to yoink means to force pull.

### Special thanks

Special thanks to OpenAI and ChatGPT for the help with implementing this wonderful command. 
