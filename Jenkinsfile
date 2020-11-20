pipeline{
 agent any
	print "${BRANCH_NAME}"
   stages{
   stage("develop"){
	   when{
	   expression {
        return env.BRANCH_NAME == 'develop';
        }
	   }
    
    steps{
	  print "develop"
	}
   }
     
   stage("master"){
	   when{
	   expression {
        return env.BRANCH_NAME == 'master';
        }
	   }
    steps{
	  print "master"
	}
   }
  }
}
