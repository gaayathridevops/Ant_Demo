pipeline {
    agent any
    stages {
        stage ('SCM'){
            steps {
                 git 'https://github.com/gaayathridevops/Ant_Demo.git'
            }
                
        }
        stage ('command') {
            steps {
                bat 'ant clean'
                bat 'ant'
            }
        }
        stage ('deploy') {
            steps {
                sh 'cp -r "C:\\Program Files (x86)\\Jenkins\\workspace\\ant again\\dist\\AntExample.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'
            }
        }
        
    }
}
