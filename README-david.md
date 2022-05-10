# Installing ohmyzsh
1. Clone this repo
2. Open `~/.zshrc` and point it to this repo via `export ZSH="/Users/davidmoe/Documents/ohmyzsh"`

# Adding plugins
Clone the repo into `/custom/plugins` folder. These are ignored in git.

Ex: `git clone https://github.com/zsh-users/zsh-autosuggestions ~/Documents/ohmyzsh/custom/plugins/zsh-autosuggestions`

# Plugins
git, z, npm, zsh-autosuggestions

# Getting latest changes from main repo
1. `git checkout master`
2. `git pull https://github.com/ohmyzsh/ohmyzsh.git master`
3. Rebase onto the branch david-custom-changes

# References
* Plugins: https://towardsdatascience.com/trick-out-your-terminal-in-10-minutes-or-less-ba1e0177b7df 