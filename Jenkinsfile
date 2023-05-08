pipeline {
	agent any
    environment {
        AUTHOR = "Mansur Efendi"
        EMAIL = "kheva@gmail.com"
    }

    options {
        disableConcurrentBuilds()
        timeout(time:10, unit: 'SECONDS')
    }
	stages {
        stage ("Build") {
            steps {
                echo ("Build")
                echo("Start Job: : ${env.JOB_NAME}")
                echo("Start Build: : ${env.BUILD_NUMBER}")
                echo("Branch Name: : ${env.BRANCH_NAME}")
                echo ("Author : ${AUTHOR}")
                sleep(20)
            }
        }

        stage ("Deploy"){
            steps {
                echo ("Deploy")  
                sleep(20)            
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
