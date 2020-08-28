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
                    echo "MAVEN_HOME = ${MAVEN_HOME}"
                '''
            }
        }
         stage('Deliver for development') {
            when {
                branch 'develop' 
            }
            steps {
                echo "DEVELOPMENT BRANCH"
            }
        }
         stage('Deliver for Production') {
            when {
                branch 'production' 
            }
            steps {
               echo  "PRODUCTION BRANCH"
            }
        }
    }
}
