pipeline {
    agent {
	    node {
	        label 'master'
	    }
    }
    stages {
        stage('build all') {
            steps {
                build job: 'sub_project', parameters: [string(name: 'THIS_PROJECT_DIR', value: 'dir'), string(name: 'THIS_PROJECT_NAME', value: 'test_name'), string(name: 'THIS_PROJECT_WEB_PORT', value: '8080'), string(name: 'THIS_MAVEN_PROFILE', value: 'pro')]
            }
        }
    }
}