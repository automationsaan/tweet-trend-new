pipeline {
    agent {
        node {
            label 'maven'
        }
    }
    environment {
        JAVA_HOME = "/usr/lib/jvm/java-21-openjdk-amd64"
        PATH = "/opt/apache-maven-3.9.9/bin:$JAVA_HOME/bin:$PATH"
    }
    stages {
        stage('Build') {
            steps {
                echo "JAVA VERSION:"
                sh 'java -version'
                echo "MAVEN VERSION:"
                sh 'mvn -version'
                echo "----------- build started ----------"
                sh 'mvn clean package'
                echo "----------- build completed ----------"
            }
        }
    }
}