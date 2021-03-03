pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install peclinic-app redchirov  --set image.repository=registry.hub.docker.com/redchir/redchirov:14 --set image.tag=1'
              			
            }           
        }
    }
}
