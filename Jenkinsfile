pipeline {
    //Agent can also be a docker 
    agent any 
 
    tools {nodejs "recent_node"}
 
    stages{
        //Installing dependencies
        stage('checkout'){
            steps{
                    sh 'node -v'
                    sh 'npm -v'
            }
        }
        stage('Testing'){
            steps{
                    sh 'npm test'
            }
        }
    }     
}
