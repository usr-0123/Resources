`install pnpm` globally using the command
```
iwr https://get.pnpm.io/install.ps1 -useb | iex
```
install `node`
install `git`
install `vscode`
register vscode with github:
```
git config --global user.name "Your Name"
```
```
git config --global user.email "your_email@example.com"
```
checking the `linked repository` in vscode 
```
git remote get-url origin
```
`remove/unlink repo` 
```
git remote remove origin
```

# Docker
## MSSQL server in docker
### Pull an image
docker pull mcr.microsoft.com/mssql/server:2022-latest

### Running
docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD={PASSWORD}" -p 1433:1433 -d --name dev-sqlserver mcr.microsoft.com/mssql server:2022-latest