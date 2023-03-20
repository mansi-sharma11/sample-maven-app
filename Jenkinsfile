pipeline {
    agent any
    
    stages {
        stage('Compile') {
            steps {
                withMaven( maven: 'Maven'){
                sh 'mvn compile'
            }
        }
    }
         stage('Test') {
            when {
                not {
                    failed()
                }
            }
            steps {
                sh 'mvn test'
            }
        }
}
}
