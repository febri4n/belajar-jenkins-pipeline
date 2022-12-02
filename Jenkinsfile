pipeline {
    agent {
    	node {
	    label "linux && java11"
	}
    }
    stages {
        stage("Hello") {
            steps {
                echo "Hello Pipeline!"
            }
        }
    }
    post {
	always {
	    echo "I will always Hello again!"
	}	
	success {
	    echo "Yay, success"
	}
	failure {
	    echo "Oh no, failure"
	}
	cleanup {
	    echo "Don't cate success or error"
	}
    }
}
