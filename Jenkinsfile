pipeline{
    agent {
        node {
            label "valaxy"
        }
    }
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
        stage('build') {
            steps{
                echo "------------ build started ---------"
                sh 'mvn clean install -Dmaven.test.skip=true'
                echo "------------ build completed ---------"
        }
      }
    }
}
