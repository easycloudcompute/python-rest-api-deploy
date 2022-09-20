pipeline {
	agent any
    stages {
        stage('Build on AKS ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
			sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install python-app --set image.repository=reg0001.azurecr.io/reg0001/python-app --set image.tag=1'
            }           
        }
    }
}
