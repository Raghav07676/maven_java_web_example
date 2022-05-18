pipeline {
       agent any
   
       stages 
       {
       stage('Build')
       {
       steps{
       echo "Building the project..."
       withMaven(maven: 'mvn') {
            sh "mvn clean package"
        }
       }
       } 
    
       stage('Test')
       {
        steps{
       echo "Testing the project..."
       withMaven(maven: 'mvn') {
            sh "mvn clean package"
        }
       }
       }

       stage('Compile')
       {
        steps{
       echo "Compiling the project..."
       withMaven(maven: 'mvn') {
            sh "mvn clean package"
        }
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
