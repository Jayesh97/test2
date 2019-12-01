pipeline {
    //Agent can also be a docker 
    agent any 
            stages{
                //Installing dependencies
                stage('checkout'){
                    steps{
                            sh 'curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -'
                            sh 'apt-get install -y nodejs'
                            sh 'apt-get install npm'
                            sh 'npm install'
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
