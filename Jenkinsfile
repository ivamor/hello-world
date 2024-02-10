pipeline {
  agent any
  stages {
    stage('Build') {
    	steps {
    		retry(3) {
    			sh './flakey-deploy.sh'
    		}
    
    		timeout(time: 3, unit: 'SECONDS') {
    			sh './health-check.sh'
    		}
    	}
    }
  }    
} 
