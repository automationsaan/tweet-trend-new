pipeline {
    agent {
        node {
            label 'maven'
        }
    }

// Create environment variable for Maven path
environment {
  PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
}

script {
  echo "----------- build started ----------"
  sh 'java -version'
  sh 'mvn -version'
  // sh 'mvn clean package'
  echo "----------- build completed ----------"
  }

  // stages {
  //   stage('Build') {
  //     steps {
  //       script {
  //         echo "----------- build started ----------"
  //         sh 'mvn clean package'
  //         echo "----------- build completed ----------"
  //       }
  //     }
  //   }
  // }
}