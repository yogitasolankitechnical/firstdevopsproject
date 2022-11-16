pipeline {
    agent any

    stages {
        stage('Validate') {
            steps {
                echo 'Building..'
		sh '/usr/share/maven/bin validate'
            }
        }
        stage('Build') {
            steps {
                echo 'Testing..'
		sh '/usr/share/maven/bin package'
            }
        }
        stage('Test') {
            steps {
                echo 'Deploying....'
		sh '/user/share/maven/bin test'
            }
        }
    }
}
