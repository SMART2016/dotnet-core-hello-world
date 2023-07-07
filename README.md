## Semver

- Enable conventional commit for the git repository
	- https://medium.com/yasser-dev/automate-and-enforce-conventional-commits-for-net-based-projects-a322be7a1eb7
- Enforce branch creation rules to follow below conventions:
	- release/*
	- feature/*
	- bugfix/*
- Merging branches to main or dev keeping the commit history intact
- Automating Versioning and Release:
	- https://blog.antosubash.com/posts/automatic-version-and-release

## Install Husky for commit message linting
- rm -rf .git/hooks
- dotnet tool install --global Husky

### Adding first git hook
- dotnet husky add pre-commit -c "echo 'Husky.Net is awesome!'"
- git add .husky/pre-commit
- chmod ug+x .husky/*