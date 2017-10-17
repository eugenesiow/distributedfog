## Install

1. Install Hugo e.g. `brew install hugo`
2. `git clone https://github.com/eugenesiow/distributedfog.git`
3. `cd distributedfog`
4. Create a public folder with the gh-pages branch with `git worktree add -B gh-pages public origin/gh-pages`
5. Build the static public folder with Hugo and commit the gh-pages branch with `./commit.sh`
6. Push the gh-pages branch to github with `./publish.sh`
