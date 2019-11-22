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
			        def map = [ name:'test2',id='2' ]
			        map.each{
			            stage(it.name){
			                echo it.key+it.value
			            }
			        }
			    }
		    }
	    }
    }
}