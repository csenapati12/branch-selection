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
	            tag1= 'Test********** env.BRANCH_NAME.$tag ????????????'
			    echo "${tag}"
		    }
            }
        }
        stage('2  develop') {
		
            when {
                branch 'develop'
            }
            steps {
             // tag = VersionNumber(projectStartDate: '2017-05-22', versionNumberString: 'develop.1.0.v${BUILDS_ALL_TIME}', versionPrefix:'',  worstResultForIncrement:'SUCCESS')
             // echo "${tag}"
		    echo "Test********** ${env.BRANCH_NAME} ?????????  ${env.BRANCH_NAME}"
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
