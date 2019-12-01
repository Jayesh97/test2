pipeline {
    //Agent can also be a docker 
    agent any 
            stages{
                //Installing dependencies
                stage('checkout'){
                    steps{
                            sh 'apt-get install -y nodejs'
                    }
                }
                stage('checkout'){
                    steps{
                            sh 'npm install'
                    }
                }
                stage('Testing'){
                    steps{
                            sh 'npm test'
                    }
                }
            }     
}
