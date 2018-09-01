pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
					echo 'maven building'
					mvn clean install -DskipTests
			}
        }
        stage('Test') {
            steps {
                echo 'Testing..'
				mvn test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
