# mvntree
![mvntree](mvntree.png)

## About
This is a small awk script to prettify the command [`mvn dependency:tree`](https://en.wikipedia.org/wiki/Apache_Maven). It will turn the ascii tree from the crude form that mvn outputs into something a little prettier. The different columns in the dependencies will have nice colours applied to them. Finally, the superfluous "[INFO] " at the start of each line is removed to save space.

## Installation
This acts as shell alias. You have two ways of loading the command:
1. You can either copy the content of the file '.mvntree' into your ~/.zshrc or ~/.bashrc file.
2. You can load the file directly. Assuming you have placed '.mvntree' in your home folder, you can place the following in ~/.zshrc:

```
source $HOME/.mvntree
```

In ~/.bashrc:

```
if [ -f ~/.mvntree ]; then
    . ~/.mvntree
fi
```

You can now use the command `mvntree` and enjoy the prettiness.
