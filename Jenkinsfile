pipeline{

       agent any
       tools{
               maven 'maven'
       }
       stages {
       
              stage ('Compile Stage'){
                       steps{
                              bat 'mvn clean compile'
                       }
              }

              stage ('Testing Stage'){
                       steps{
                              bat 'mvn test'
                       }
              }
       
              stage ('Sonarqube deployment Stage'){
                       steps{
                              bat 'mvn sonar:sonar'
                       }
              
              }
            
       }

}