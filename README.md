# ✅Connecting jenkins to gitlab through access tokens😎

### -> 🤦🏻‍♂️Install plugins in Jenkins Gitlab API and Gitlab Plugin🤞🏻
### -> 🤳🏻Create new access Token in gitlab with API and read and write marked ( Copy and save it you'll get it again )
### -> In manage Jenkins Add Git specs and test the connection 👩🏻‍❤️‍👨🏻
### -> create a new credential  in jenkins Using this token and Username of gitlab
          1) use username and password option 🪢
          2) Give your username of gitlab account🧥
          3) Give the token generated from gitlab in place of Password (💔 Not the original gitlab account password )
          4) After giving everything save ( ❤️‍🩹 Always Remember to save the process in jenkins )
### -> Create a new job in jenkins Using pipeline❣💞
### -> run a basic helloworld command in pipeline 💓( You'll get the code which is in built Inside pipeline section -> pipeline script top right you'll get the drop down click on hello world )
### -> Save and run Build 💘
### -> After building turns green click on configure -> pipeline -> pipeline Syntax.
### -> in the sample steps dropdown select Checout from version control🤭
### -> Give details of repository and select credentials -> click on generate syntax👶🏻
### -> copy and paste the syntax
        stages {
        stage('Hello') {
            steps {
                👉🏻👉🏻👉🏻  PASTE IT HERE
            }
        }
### -> SAVE AND APPLY 🤵🏻👰🏻‍♀️
### -> build it again ( Yup.. You configured gitlab 👍 )
### -> hope build stage turns green 💚

## 🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢🪢

# ✅Installing Gradle on Jenkins ( I would like to give gradle path to jenkins by installing it on my os❗️ )
### I deployed jenkins on AWS EC2 ( use your pem file and IP adress given by instance )
          ssh -i file_name.pem ec2user@192.168.1.1
### after logging in Install gradle ( usually there will be problem to install directtly using yum follow this method )
           wget https://github.com/gradle/gradle/releases/download/v8.5.0/gradle-8.5-bin.zip
### it will download zip file make sure u give your own version
           unzip gradle-8.5-all.zip
### Check gradle version to verify installation
          gradle --version 
### to add to environment variable and its path
          sudo mv gradle-8.5 /opt/gradle
          export PATH=$PATH:/opt/gradle/bin
### check Path variables for confirmation 
          echo $PATH | grep gradle
### copy the path to gradle usually it will be in form of 
          /opt/gradle
###  open jenkins in browser 
### 👉🏻 manage jenkins
### 👉🏻 tools
### 👉🏻 gradle installation ( it will be visible only if you have installed gradle plugin)
### 👉🏻 uncheck automatic installation it will ask the GRADLE_HOME path paste the copied path
### 👉🏻 Save and apply  🪢
## Done👍    
