pipeline{

       agent any
       tools{
               maven 'maven'
       }
       stages {
       
              stage ('Compile Stage'){
                       steps{
                              bat 'mvn clean install'
                       }
              }

       
              stage ('Sonarqube deployment Stage'){
                       steps{
                              bat 'mvn sonar:sonar'
                       }
              
              }
            
       }

}