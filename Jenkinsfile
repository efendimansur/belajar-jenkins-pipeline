pipeline {
	agent any
	stages {
        stage ("Hello") {
            steps {
                echo ("Update Hello Pipeline")
            }
        }
	}

    post {
        always {
            echo "I will always say Hello again!"
        }
    }
}
