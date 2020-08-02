# automatic_build_number
Add build number in your package.json, 
sync with your git commits after push

## Shell version
- Put file called pre-commit in .git/hooks/
- Your package.json need to have "build" tag as shown in package.json file:
```
{
  "name": "myapp",
  "version": "1.0.0",
  "build": 2,
  ...
}
```
## Node.js version
- Create a file called pre-commit in .git/hooks/ with :
```
node pre-commit.js
```
- Put file called pre-commit.js in your root folder
- You just need to have a valid package.json file in your root folder