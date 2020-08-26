pipeline {
    agent any
    tools { 
        maven 'Maven 3.5.2' 
        jdk 'JDK8' 
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${MAVEN_HOME}"
                ''' 
            }
        }

        stage ('Build') {
            steps {
                echo 'This is a sample pipeline.'
            }
        }
    }
}
