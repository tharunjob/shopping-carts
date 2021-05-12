pipeline{
  
    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven ‘maven’
    }


    stages{
        stage('build'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('package'){
            steps{
                sh 'mvn package'
            }
        }
    }

    post{
        always{
            echo 'this pipeline is for shopping-carts application...'
        }

    }

}
