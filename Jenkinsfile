// Declarative //
pipeline {
    agent any
    environment {
        CC = 'clang'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Build'
                echo 'Params:'
                echo "BRANCH_NAME: ${env.BRANCH_NAME}"
                echo "CHANGE_ID: ${env.CHANGE_ID}"
                echo "CHANGE_URL: ${env.CHANGE_URL}"
                echo "CHANGE_TITLE: ${env.CHANGE_TITLE}"
                echo "CHANGE_AUTHOR: ${env.CHANGE_AUTHOR}"
                echo "CHANGE_AUTHOR_DISPLAY_NAME: ${env.CHANGE_AUTHOR_DISPLAY_NAME}"
                echo "CHANGE_AUTHOR_EMAIL: ${env.CHANGE_AUTHOR_EMAIL}"
                echo "CHANGE_TARGET: ${env.CHANGE_TARGET}"
                echo "BUILD_NUMBER: ${env.BUILD_NUMBER}"
                echo "BUILD_ID: ${env.BUILD_ID}"
                echo "BUILD_DISPLAY_NAME: ${env.BUILD_DISPLAY_NAME}"
                echo "JOB_NAME: ${env.JOB_NAME}"
                echo "JOB_BASE_NAME: ${env.JOB_BASE_NAME}"
                echo "BUILD_TAG: ${env.BUILD_TAG}"
                echo "EXECUTOR_NUMBER: ${env.EXECUTOR_NUMBER}"
                echo "NODE_NAME: ${env.NODE_NAME}"
                echo "NODE_LABELS: ${env.NODE_LABELS}"
                echo "WORKSPACE: ${env.WORKSPACE}"
                echo "JENKINS_HOME: ${env.JENKINS_HOME}"
                echo "JENKINS_URL: ${env.JENKINS_URL}"
                echo "BUILD_URL: ${env.BUILD_URL}"
                echo "JOB_URL: ${env.JOB_URL}"
                // sh 'make'
            }
        }

        stage('Example') {
            environment {
                DEBUG_FLAG = '-g'
            }
            steps {
                sh 'printenv'
            }

        }

        stage('Test') {
            steps {
                echo 'Test'
                // sh 'make check'
                // junit 'reports/**/*.xml'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy'
                // sh 'make publish'
            }
        }
    }
}

// Script //
// node {
//     stage('Build'){
//                 echo 'Build'
//                 // sh 'make'
//     }

//     stage('Test'){
//         echo 'Test'
//         // sh 'make check'
//         // junit 'reports/**/*.xml'
//     }

//     stage('Deploy'){
//         echo 'Deploy'
//         // sh 'make publish'
//     }    
// }