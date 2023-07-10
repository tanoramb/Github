## Repository
Create a new repository on the command line
```
echo "# Github" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/tanoramb/Github.git
git push origin main
```
Push an existing repository from the command line
```
git remote add origin https://github.com/tanoramb/Github.git
git branch -M main
git push origin main
```
When creating a file and then uploading to Github
```
create file.txt
git add -A   | git add file.txt
git commit -m "message"
git push origin main
```

## Credentials
1. Create token classic at [your settings](https://github.com/settings/apps)
2. Grab and copy de Token
3. Install [GCM - Github credential manager](https://github.com/git-ecosystem/git-credential-manager/blob/release/docs/install.md)
   <br>
   Linux deb package (ubuntu):
   ```
   sudo dpkg -i <path-to-package>
   ```
5. Run the following command:
   ```
   git config --global credential.helper store
   ```
6. When doing `git push origin main` enter your credentials:
   ```
   Username for 'https://github.com': username at github.com
   Password for 'https://tanoramb@github.com': [Paste the Token]
   ```
7. Your credentials now are stored in the system
   
   
