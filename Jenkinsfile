pipeline {
    agent any

    stages {
        stage("Build"){
            steps {
                script {
                    sh "mvn package -DskipTests=true"
                    sh "mvn release:prepare"
                    sh "mvn release:perform"
                }
            }
        }
    }
}
