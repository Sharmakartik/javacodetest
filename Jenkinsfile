  
@Library('kartiklibrary') _
 
 pipeline {
    agent any
      tools {
         jdk 'java'
         maven 'maven'
             }
          stages {
             stage('Build') { 
                         steps {
               
                                   bat 'mvn -B -DskipTests clean package'      
                                   echo """" build1 """
                                   echo "build1currentResult: ${currentBuild.currentResult}"
                           script{
                              log.info'hello'
                              log.warning'red alert'
                              build 'package'
                           
                           }
                                 
        
                               }
                             }
                          }
 }
                 
        
