pipeline {
    //Agent can also be a docker 
    agent any 
            stages{
                //Installing dependencies
                stage('checkout'){
                    steps{
			                sh 'apt-get install nodejs'
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
