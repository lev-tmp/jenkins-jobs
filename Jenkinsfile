// Declarative //
// pipeline {
//     agent any

//     stages {
//         stage('Build') {
//             steps {
//                 echo 'Build'
//                 // sh 'make'
//             }
//         }

//         stage('Test') {
//             steps {
//                 echo 'Test'
//                 // sh 'make check'
//                 // junit 'reports/**/*.xml'
//             }
//         }

//         stage('Deploy') {
//             steps {
//                 echo 'Deploy'
//                 // sh 'make publish'
//             }
//         }
//     }
// }

// Script //
node {
    stage('Build'){
                echo 'Build'
                echo 'Params:'
                echo "${params.BRANCH_NAME}"
                echo "${params.CHANGE_ID}"
                echo "${params.CHANGE_URL}"
                echo "${params.CHANGE_TITLE}"
                echo "${params.CHANGE_AUTHOR}"
                echo "${params.CHANGE_AUTHOR_DISPLAY_NAME}"
                echo "${params.CHANGE_AUTHOR_EMAIL}"
                echo "${params.CHANGE_TARGET}"
                echo "${params.BUILD_NUMBER}"
                echo "${params.BUILD_ID}"
                echo "${params.BUILD_DISPLAY_NAME}"
                echo "${params.JOB_NAME}"
                echo "${params.JOB_BASE_NAME}"
                echo "${params.BUILD_TAG}"
                echo "${params.EXECUTOR_NUMBER}"
                echo "${params.NODE_NAME}"
                echo "${params.NODE_LABELS}"
                echo "${params.WORKSPACE}"
                echo "${params.JENKINS_HOME}"
                echo "${params.JENKINS_URL}"
                echo "${params.BUILD_URL}"
                echo "${params.JOB_URL}"
                // sh 'make'
    }

    stage('Test'){
        echo 'Test'
        // sh 'make check'
        // junit 'reports/**/*.xml'
    }

    stage('Deploy'){
        echo 'Deploy'
        // sh 'make publish'
    }    
}


