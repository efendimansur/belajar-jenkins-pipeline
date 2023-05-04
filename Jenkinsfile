pipeline {
	agent any
    environment {
        AUTHOR = "Mansur Efendi"
        EMAIL = "kheva@gmail.com"
    }
	stages {
        stage ("Build") {
            steps {
                echo ("Build")
                echo("Start Job: : ${env.JOB_NAME}")
                echo("Start Build: : ${env.BUILD_NUMBER}")
                echo("Branch Name: : ${env.BRANCH_NAME}")
                echo ("Author : ${AUTHOR}")
            }
        }

        stage ("Test") {
            steps {                                         
            }
        }

        stage ("Deploy"){
            steps {
                echo ("Deploy")              
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
