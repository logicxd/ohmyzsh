# Installing ohmyzsh
1. Clone this repo
2. Open `~/.zshrc` and point it to this repo via `export ZSH="/Users/davidmoe/Documents/ohmyzsh"`
  1. If you don't see `~/.zshrc`, you can create one.

# Adding plugins
Clone the repo into `/custom/plugins` folder. These are ignored in git.

Ex: `git clone https://github.com/zsh-users/zsh-autosuggestions ~/Documents/ohmyzsh/custom/plugins/zsh-autosuggestions`

# Plugins
git, z, npm, zsh-autosuggestions

# Powerlevel10k
Some theme customization is done inside of `~/.p10k.zsh`
```
    if [[ -n $VCS_STATUS_LOCAL_BRANCH ]]; then
      local branch=${(V)VCS_STATUS_LOCAL_BRANCH}
      # If local branch name is at most 32 characters long, show it in full.
      # Otherwise show the first 12 … the last 12.
      # Tip: To always show local branch name in full without truncation, delete the next line.

      # DM: commented out below
      # (( $#branch > 32 )) && branch[13,-13]="…"  # <-- this line
      # res+="${clean}${(g::)POWERLEVEL9K_VCS_BRANCH_ICON}${branch//\%/%%}"
    fi
```

# Getting latest changes from main repo
1. `git checkout master`
2. `git pull https://github.com/ohmyzsh/ohmyzsh.git master`
3. Rebase onto the branch david-custom-changes

# References
* Plugins: https://towardsdatascience.com/trick-out-your-terminal-in-10-minutes-or-less-ba1e0177b7df 