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
}
}
