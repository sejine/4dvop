pipeline {
    agent any
  
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
        stage("Build and start") {
            steps {
		script{
		sh "docker-composer build"
                sh "docker-compose up -d"
                waitUntilServicesReady
                
                }
            }
            
        }
}
        
        
 

