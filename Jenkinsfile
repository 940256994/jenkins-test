def map = [:]
map.put('name','caoran')
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