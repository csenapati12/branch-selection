pipeline{
 agent any
stages{
   stage("develop"){
	   when{ branch 'develop' }    
    steps{
	  print "develop"
	}
    }
     
   stage("master"){
	  when{ branch 'master' }
        steps{
	  print "master"
	}
    }
  }
}
