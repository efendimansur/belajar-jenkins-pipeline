pipeline {
	agent any
	stages {
        stage ("Build") {
            steps {
                echo ("Build")
                sleep(10)
                echo("Start Job: : ${env.JOB_NAME}")
                echo("Start Build: : ${env.BUILD_NUMBER}")
                echo("Branch Name: : ${env.BRANCH_NAME}")
            }
        }

        stage ("Test") {
            steps {
                script {
                    def data = [
                        "firstName": "Mansur",
                        "lastName": "Efendi"
                    ]
                    writeJSON(file: "data.json", json:data)
                }                              
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
