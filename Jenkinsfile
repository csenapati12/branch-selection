pipeline {
    agent any
    stages {
        stage('1') {
            steps {
                echo 'Hello World'
            }
        }
        stage('2  develop') {
            when {
                branch 'develop'
            }
            steps {
                echo 'develop'
            }
        }
 stage('3 master') {
            when {
                branch 'master'
            }
            steps {
                echo 'master'
            }
        }	    
	    
    }
}
