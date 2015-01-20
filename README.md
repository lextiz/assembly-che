### Clone the Repository
```sh
git clone https://github.com/codenvy/assembly-che.git
cd assembly-che
```
### Run the script, that clones all Codenvy repositories
To run the script you need to generate an access token in your github account
https://help.github.com/articles/creating-an-access-token-for-command-line-use/

Set github token environment variable
```sh
export GITHUB_TOKEN=[paste generated token]
```

Run the  script
```sh
./clone_codenvy.sh
```

### Build and Run Che
```sh
mvn clean install
./che [ start | stop ]
```

Che will be available at ```localhost:8080```