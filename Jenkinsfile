pipeline{
    agent any
    stages{
        stage('parallel work'){
            parallel{
                stage('test'){
                    steps{
                        sh 'mvn test'
                    }
                }
                stage('build'){
                    steps{
                        sh 'mvn clean package -DskipTests'
                    }
                }
            }
            
        }
       
    }
}
