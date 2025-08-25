pipeline{
    agent 
        docker{
            image 'cypress/browsers:lastest'
            args '--entrypoint='
        }
    stages{
        stage('test3'){ 
            steps{
                echo 'hello jenkins'
            }
        }         
        stage('test1'){ 
            steps{
                echo 'install npm'
                sh 'npm ci'
            }
        } 
        stage('test2'){ 
            steps{
                echo 'hello from jenkinsfile'
                sh 'npx run ci --browser chrome'
            }
        }  
    }
}