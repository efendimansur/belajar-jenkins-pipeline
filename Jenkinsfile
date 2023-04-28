pipeline {
	agent any
	stages {
        stage ("Build") {
            steps {
                echo ("Build")
                sleep(5)
                echo("Build")
            }
        }

        stage ("Test") {
            steps {
                echo ("Test")
                sleep(5)
                echo("Test2")                
            }
        }

        stage ("Deploy"){
            steps {
                echo ("Deploy")
                sleep(5)
                echo("Deploy2")                
            }
        }
	}

    post {
        always {
            echo "I will always say Hello again!"
        }

        success {
            echo "sukses"
        }

        failure {
            echo "gagal"
        }
    }
}
