### Configure Tooling
 Configure information for all local repositories |
 :--- |
 `$ git config --global user.name "[name]"` <br> Sets the name you want attached to your commit transactions |
 `$ git config --global user.email "[email address]"` <br> Sets the email you want attached to your commit transactions |
 `$ git config --global color.ui auto` <br> Enables helpful colorizatoin of command line output |

### Create Repositories
 Start a new repository or obtain one from an existing URL |
 :--- |
 `git init [project-name]` <br> creates a new local repository with the specified name |
 `$ git clone [url]` <br> Downloads a project and its entire version history |

### Make Changes
 Review edits and craft a commit transaction |
 :--- |
 `$ git status` <br> Lists all new or modified files to be committed |
 `$ git diff` <br> Shows file differences not yet staged |
 `$ git add [file]` <br> Snapshots the file in preparation for versioning |
 `$ git diff --staged` <br> Shows file differences between staging and the last file version |
 `$ git reset [file]` <br> Unstages the file, but preserves its contents |
 `$ git commit -m "[descriptive message]"` <br> Records file snapshots permanently in version history |

### Group Changes
 Name a series of commits and combine completed efforts |
 :--- |
 `$ git branch` <br> Lists all local branches in the current repository |
 `$ git branch [branch-name]` <br> Creates a new branch |
 `$ git checkout [branch-name]` <br> Switches to the specified branch and updates the working directory |
 `$ git merge [branch]` <br> Combines the specified branch's history into the current branch |
 `$ git branch -d [branch-name]` <br> Deletes the specified branch |

### Refactor Filenames
 Relocate and remove versioned files |
 :--- |
 `$ git rm [file]` <br> Deletes the file from the working directory and stages the deletion |
 `$ git rm --cached [file]` <br> Removes the file from the version control but preserves the file locally |
 `$ git mv [file-original] [file-renamed]` <br> Changes the file name and prepares it for a commit |

### Suppress Tracking
 Exclude temporary files and paths |
 :--- |
 ```*.log
 build/
 temp-*``` <br> A text file named .gitignore suppresses accidental versioning of files and paths matching the specific patterns |
 `$ git ls-files --other --ignored --exclude-standard` <br> Lists all ignored files in this project |


