pipeline {
    agent any
	 environment {
        branch = 'env.BRANCH_NAME'
      
    }
    stages {
        stage('1') {
            steps {
		    echo 'Hello World ${params.branch}'
		    echo 'Hello World env.BRANCH_NAME'
		    print  env.BRANCH_NAME
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
