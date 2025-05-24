pipeline {
    agent {
        node {
            label 'maven'
        }
    }
    environment {
        PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
    }
    stages {
        stage('Build') {
            steps {
                echo "----------- build started ----------"
                sh 'mvn clean package'
                echo "----------- build completed ----------"
            }
        }
    }
}