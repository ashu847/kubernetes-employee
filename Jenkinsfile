pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install employee-app petclinic  --set image.repository=registry.hub.docker.com/ashu847/employee-management-react --set image.tag=1.0'
              			
            }           
        }
    }
}
