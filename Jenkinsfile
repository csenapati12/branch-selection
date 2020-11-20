pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example develop') {
            when {
                branch 'develop'
            }
            steps {
                echo 'develop'
            }
        }
 stage('Example master') {
            when {
                branch 'master'
            }
            steps {
                echo 'master'
            }
        }	    
	    
    }
}
