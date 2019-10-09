  
@Library('kartiklibrary') _
 def h= new Utilities(this)
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
                                       h.mvn'clean'
                                       build()
                                          } 
                                  }
        
                               }
                     }
     }
        
                 
        
