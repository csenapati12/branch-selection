pipeline{
 
stages{
   stage("develop"){
	   agent any
	   when{ branch 'develop' }    
    steps{
	  print "develop"
	}
    }
     
   stage("master"){
	   agent any
	  when{ branch 'master' }
        steps{
	  print "master"
	}
    }
  }
}
