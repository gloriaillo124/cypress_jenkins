pipeline {
    agent {
        docker {
            image 'cypress/browsers:latest'
            args '--entrypoint='
        }
    }
    stages {
        stage('test3') { 
            steps {
                echo 'hello jenkins'
            }
        }         
        stage('test1') { 
            steps {
                echo 'install npm'
                sh 'npm ci'
            }
        } 
        stage('test2') { 
            steps {
                echo 'hello from jenkinsfile'
                sh 'npm run ci -- --browser chrome'
            }
        }  
    }
}
