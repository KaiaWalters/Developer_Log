
# 🗓️ Developer Log

## 🛠 What I Worked On
- Investigated Docker installation and path configuration issues
- Debugged dependency versioning conflicts in the project (specifically `@clerk/shared@3.27.0`)
- Resolved Git merge conflicts and revisited rebasing workflows
- Reviewed TypeScript path mapping configuration and its impact across branches

## 📚 What I Learned
**Docker & Terminal Path Management:**
- How to detect which Docker installation is being executed (`type docker`, `which -a docker`)
- Difference between npm-installed Docker CLI and Docker Desktop
- How terminal commands connect to executable paths
- How to verify app installation: `ls /Applications/Docker.app`
- How to modify PATH for Docker Desktop: `export PATH="$PATH:/Applications/Docker.app/Contents/Resources/bin/"`
- [Reference: Docker path troubleshooting](https://www.youtube.com/watch?v=Tpyh88yymaA)

**NPM Dependency Management:**
- How to override nested dependency versions using `overrides` in `package.json`
- How to view all project packages and versions: `npm ls --depth=0`
- What "extraneous" means in `package-lock.json` (package installed but not defined in dependencies)
- [Reference: Overriding nested NPM dependencies](http://stackoverflow.com/questions/15806152/ddg#48524488)

**Git:**
- Revisited rebasing and merging workflows

**Other Tools:**
- `sed -i` command for modifying files directly from terminal
- [Reference: Mastering text manipulation with sed](https://www.linuxjournal.com/content/mastering-text-manipulation-sed-command)
- `npm ls -- depth = 0 ` for viewing all packages withing a project and their versions


## ✅ What Went Well
- Successfully diagnosed and resolved Docker path configuration issues
- Identified the root cause of path-related execution problems
- Expanded knowledge of dependency management tooling

## 🚧 What Blocked Me
- Multiple versions of `@clerk/shared@3.27.0` causing conflicts in the project
- Cursor AI not accounting for dependency interactions when suggesting changes, leading to conflicting packages
- TypeScript path mapping discrepancies between branches (aliasing `src` as `./*`) causing import resolution issues

## 🔜 Next Steps
- Investigate specific packages causing version conflicts in more depth
- Improve package.json versioning strategy between production deploys
- Establish better practices for versioning `tsconfig.json` and highlighting changes in PR descriptions
- Explore sed commands further for potential scripting automation

## 📝 Notes / Reflections
- Working with a large, fast-moving team requires extra attention to configuration files that impact the entire project (like `tsconfig.json`)
- Need to be more mindful of how path mapping and TypeScript config changes affect other team members
- Dependency management is more complex than just resolving conflicts in `package.json` – understanding how packages interact in the same environment is crucial
- Terminal path management and understanding where commands execute from is fundamental knowledge that can prevent confusing debugging sessions
