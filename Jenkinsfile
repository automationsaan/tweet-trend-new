pipeline {
    agent {
        node {
            label 'maven'
        }
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