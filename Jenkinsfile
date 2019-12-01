pipeline {
    //Agent can also be a docker 
    agent any 
            stages{
                //Installing dependencies
                stage('checkout'){
                    steps{
                            sh 'apt-get install -y nodejs'
                            sh 'ls'
                    }
                }
                //This stage performs unittest
                stage('Testing'){
                    steps{
                            sh 'npm test'
                    }
                }
            }     
}
