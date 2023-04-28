pipeline {
	agent any
	stages {
        stage ("Build") {
            steps {
                echo ("Build")
                sleep(10)
                echo("Build")
            }
        }

        stage ("Test") {
            steps {
                echo ("Test")
                sleep(15)
                echo("Test2")
                sh("/usr/bin/ping -c 4 google.com")                
            }
        }

        stage ("Deploy"){
            steps {
                echo ("Deploy")
                sleep(20)
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
