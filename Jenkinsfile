pipeline{
    agent 
    docker{
        image 'cypress/browsers:lastest'
        args '--entrypoint='
    }
    stages{
        stage('test1'){ 
            steps{
                echo 'install npm'
                sh 'npm install'
            }
        } 
        stage('test2'){ 
            steps{
                echo 'hello from jenkinsfile'
                sh 'npx run ci'
            }
        }  
         stage('test3'){ 
            steps{
                echo 'hello every body'
            }
        }         
    }
}