pipeline {
    agent { docker { image 'maven:3.9.6-eclipse-temurin-17-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                    mvn -help
                    echo "Hello saumya"
                '''
            }
        }
    }
}