
## GIT 

### gitignore for macos

        # General
        .DS_Store
        .AppleDouble
        .LSOverride

        # Icon must end with two \r
        Icon


        # Thumbnails
        ._*

        # Files that might appear in the root of a volume
        .DocumentRevisions-V100
        .fseventsd
        .Spotlight-V100
        .TemporaryItems
        .Trashes
        .VolumeIcon.icns
        .com.apple.timemachine.donotpresent

        # Directories potentially created on remote AFP share
        .AppleDB
        .AppleDesktop
        Network Trash Folder
        Temporary Items
        .apdisk

### Git commands

        create project : git init
        clone repo : git clone <repo-url>
        check status : git status
        add files to staging area : git add <file-name> OR git add .
        check changes between current dir and staging area : git diff
        create a commit : git commit -m 'your-message'

        check all branches : git branch
        create a new branch : git branch <new-branch-name>
        point to a new branch : git checkout <branch-name>
        Delete a branch : git branch -d <branch-name>

        pull new updates and commits from remote branch : git fetch origin/master
        git pull performs git fetch followed by git merge where as git fetch does not effect the local repo 


        check commit history : git log


## Run quarkus with quarkus cli 

- install quarkus :

        curl -Ls https://sh.jbang.dev | bash -s - trust add https://repo1.maven.org/maven2/io/quarkus/quarkus-cli/
        curl -Ls https://sh.jbang.dev | bash -s - app install --fresh --force quarkus@quarkusio

- create a quarkus project : 
    
        quarkus create && cd code-with-quarkus 

- run app  : 

        quarkus dev

- quarkus app will be running on : 

        localhost:8080

- make changes by editing :

        src/main/java/org/acme/GreetingResource.java


## install Maven 

- refer to this link 
        
        https://www.youtube.com/watch?v=2-bt_vGkUiQ

## Run quarkus with maven 

- create starter project :

        mvn io.quarkus:quarkus-maven-plugin:1.13.3.Final:create \
        -DprojectGroupId=com.example \
        -DprojectArtifactId=quarkus-api \
        -DclassName="com.example.HelloResource" \
        -Dpath="/hello"

- change dir :

        cd <folder-name>

- run maven :

        ./mvnw compile quarkus:dev

- quarkus project will be running on :

        localhost:8080