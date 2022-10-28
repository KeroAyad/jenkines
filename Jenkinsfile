pipeline {
     agent { label 'hamada' }
    stages {

          
        
        // deploy in ubuntu agent 
         stage('Deploy') {
            steps {
                // Get some code from a GitHub repository
                sh "docker run -d -p 80:3000 kerolosayad/nodeapp2"
            }
             post{
                success{
                echo 'app deploy successfully!'
                }
            }
          
        }
    }
}
