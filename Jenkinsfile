pipeline {
    agent any
  
	stages{
		stage("build") {
                   steps {
                    script {
                    sh "docker build ./simple_api/."
		    sh "docker images"
		    sh "docker image ls"
	            sh "docker ps -s"
                }
            }
        }
        
        }
}
        
        
 

