pipeline {
    agent {
        docker {
            image 'maven:3-alpinea'
            args '-v /root/.m2:/root/.m2'
       }
    }

    stages {
        stage('Build') {
            steps { 
                sh 'mvn -B -DskipTest clean package'
            }
        }
    }
}

    
