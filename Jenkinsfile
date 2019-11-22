def map = [ name:'test2',asd='2' ]
pipeline {
    agent {
	    node {
	        label 'master'
	    }
    }
    stages {
    	stage('PRE CHECK') {
    		steps {
    			script {
			        map.each{
			            stage(it.name){
				            steps{
				                echo "${it.key}${it.value}"
				            }
			                
			            }
			        }
			    }
		    }
	    }
    }
}