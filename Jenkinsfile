pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
		post{
		always {
		emailext body: '''hello hello ,
i was executed.
''', subject: 'plan executé', to: 'oussama.louati@esprit.tn'
		}}	
        }
		
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
