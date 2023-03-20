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
                    sh "echo IN NOT BLOCK"
                }
            }
            steps {
                sh 'mvn test'
            }
        }
}
}
