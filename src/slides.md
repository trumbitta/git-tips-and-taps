class: center, middle, main-title

# git://tips+taps

---
class: center, middle

# Git <span class="fa fa-heart"></span> Terminal

--
# A **good** terminal emulator

--
# A **nice** prompt

--
![](img/iterm-prompt.png)

---
class: center, middle

# Git <span class="fa fa-heart"></span> Colors

---
class: middle

.center[
# Git <span class="fa fa-heart"></span> Colors
]

```bash
# ~/.gitconfig

[color]
        ui = auto
[color "branch"]
        current = yellow reverse
        local = yellow
        remote = green
[color "diff"]
        meta = yellow bold
        frag = magenta bold
        old = red bold
        new = green bold
[color "status"]
        added = yellow
        changed = green
        untracked = cyan
```

---
class: center, middle

# Git <span class="fa fa-heart"></span> Colors

![](img/status-color.png)

---
class: center, middle

# Trust `git status`

---
class: middle

.center[
# Trust `git status`
]

```bash
echo 'alias gits="git status"' >> ~/.bash_profile
```

---
class: center, middle

# Read every output message

---
class: center, middle

# Messages are helpful

---
class: center, middle

# Messages are good

---
class: center, middle

# Read every output message

---
class: center, middle

# <span class="fa fa-code-fork"></span> Always work in branches

---
class: center, middle

# 1 task <span class="fa fa-arrows-h"></span> 1 local branch

---
class: center, middle

# Atomic commits == \#win

---
class: middle

.center[
# Atomic commits == \#win
]

```bash
# add files in <path> chunk by chunk
git add -p <path>

# add everything chunk by chunk
git add -p
```

---
class: center, middle

# <span class="fa fa-frown-o"></span> Save a headache... <span class="fa fa-frown-o"></span>

---
class: center, middle

.text-smaller[
# <span class="fa fa-heart"></span> ...write good commit messages! <span class="fa fa-heart"></span>
]

```
http://chris.beams.io/posts/git-commit/
```

---
class: center, middle

# <span class="fa fa-code-fork"></span> Submit pull requests

---
class: center, middle

.text-smaller[
# Code reviews help the team <span class="fa fa-line-chart"></span> grow
]

---
class: center, middle

.text-smaller[
# Front-end developer writing PHP?

Let a back-end developer review & merge
]

---
class: center, middle

.text-smaller[
# PHP developer writing JavaScript?

Let a front-end developer review & merge
]

---
class: center, middle

# <span class="fa fa-hand-o-up"></span> Speaking of which...

---
class: middle

.center[
# <span class="fa fa-hand-spock-o"></span> Merge smart
]

```bash
git checkout <current_development_branch>

# --no-ff: never perform a fast-forward
# --log: add commit messages to the merge commit
git merge --no-ff --log <topic_branch>

# If want to be extra-careful, add
# --no-commit: perform a dry-run merge
git merge --no-ff --log --no-commit <topic_branch>

# WARNING: This will leave the repo with a half-done merge.
#          Carefully look at what `git status` says, and do it.
#
# Example: All conflicts fixed but you are still merging.
#          (use "git commit" to conclude merge)
git commit
```

---
class: code-smaller

# Resources

oh-my-git  
`https://github.com/arialdomartini/oh-my-git`

Try Git  
`https://try.github.io`

Pro Git  
`https://git-scm.com/book/en/v2`

---
class: center, middle, thanks

# Thanks!

William Ghelfi  
<span class="fa fa-github"></span> trumbitta
