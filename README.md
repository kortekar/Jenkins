# Connecting jenkins to gitlab through access tokens😎

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
