pipeline{
    agent 
    docker{
        image 'cypress/browsers:lastest'
        args '-u root'
    }
    stages{
        stage('test stage'){ 
            steps{
                echo 'hello from jenkinsfile'
                sh 'npx run ci'
            }
        }  
         stage('test'){ 
            steps{
                echo 'hello every body'
            }
        }         
    }
}