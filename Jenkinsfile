pipeline {
       agent any
   
       stages 
       {
       stage('Build')
       {
       steps{
       echo "Building the project..."
       withMaven(maven: 'mvn') {
            sh "mvn test"
        }
       }
       } 
    
       stage('Test')
       {
        steps{
       echo "Testing the project..."
       sh "mvn test"
       }
       }

       stage('Compile')
       {
        steps{
       echo "Compiling the project..."
       sh "mvn compile"
       }
       }

       stage('Deploy')
       {
        steps{
       echo "Deploying the project..."
       }
       }   
       }
}
