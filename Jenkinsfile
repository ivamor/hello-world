pipeline {
  agent any
  stages {
    stage('Build') {
    	steps {    
    		timeout(time: 3, unit: 'SECONDS') {
    			sh './health-check.sh'
    		}
    	}
    }
  }    
} 
