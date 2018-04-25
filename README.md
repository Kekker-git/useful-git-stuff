# useful-git-stuff
This is a bunch of links for useful git commands that I really need to keep track of, with mini-tutorials attached.
So, let's begin.

## Managing forks
### Rebasing a fork
[Link](https://stackoverflow.com/questions/7244321/how-do-i-update-a-github-forked-repository)  
Rebasing forks is pretty easy. You add a connection to the primary repo called "upstream", and then just rebase to that.

## Managing commits
### Deleting commits
[Link](https://github.com/dolphin-emu/dolphin/pull/6477)  
The Dolphin devs were very helpful with some of my early git work, so props to them for this one. It's mistyped, so the actual command should be
```
git reset --hard HEAD~n
```
The rest of what Lioncash wrote is covered in Squashing Commits.

### Squashing Commits
[Link](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History)  
Man, git really needs a simple `git squash` command. Basically, you take the last `n` commits you have and run `git rebase -i HEAD~n`. This will give you a text file, where you can squash commits into each other, then another text file where you can edit the commit message. This SHOULD work fine. If you want to delete commits, you'll want to look at `git reset`.

## Makefiles
https://stackoverflow.com/questions/909046/makefile-in-windows?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa
