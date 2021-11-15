properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                sh '''
                sh $WORKSPACE/script.sh
                echo "nothing is there"
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Hello World Testing' 
                sh 'pwd'
                echo  "$WORKSPACE"
                echo "$BUILD_NUMBER"
                echo "$BUILD_URL"
                echo "$JENKINS_HOME"
                echo "$BUILD_NUMBER"
            }
        }
    }
}
