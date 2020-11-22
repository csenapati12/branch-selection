pipeline {
    agent any
	 environment {
        branch = 'env.BRANCH_NAME'
      
    }
    stages {
        stage('1') {
		
            steps {
		    script{
		    echo  env.BRANCH_NAME		    
		    echo  "${env.BRANCH_NAME}"
	            tag ="336"
	            echo "Test********** ${env.BRANCH_NAME}.${tag} ????????????"
		    }
            }
        }
        stage('2  develop') {
		
            when {
                branch 'master'
            }
           steps {
		    script{
		    echo  env.BRANCH_NAME		    
		    echo  "${env.BRANCH_NAME}"
	            tag ="336master"
	            echo "Test********** ${env.BRANCH_NAME}.${tag} ????????????"
		    }
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
