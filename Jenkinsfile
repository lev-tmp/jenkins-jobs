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
                echo "${env.BRANCH_NAME}"
                echo "${env.CHANGE_ID}"
                echo "${env.CHANGE_URL}"
                echo "${env.CHANGE_TITLE}"
                echo "${env.CHANGE_AUTHOR}"
                echo "${env.CHANGE_AUTHOR_DISPLAY_NAME}"
                echo "${env.CHANGE_AUTHOR_EMAIL}"
                echo "${env.CHANGE_TARGET}"
                echo "${env.BUILD_NUMBER}"
                echo "${env.BUILD_ID}"
                echo "${env.BUILD_DISPLAY_NAME}"
                echo "${env.JOB_NAME}"
                echo "${env.JOB_BASE_NAME}"
                echo "${env.BUILD_TAG}"
                echo "${env.EXECUTOR_NUMBER}"
                echo "${env.NODE_NAME}"
                echo "${env.NODE_LABELS}"
                echo "${env.WORKSPACE}"
                echo "${env.JENKINS_HOME}"
                echo "${env.JENKINS_URL}"
                echo "${env.BUILD_URL}"
                echo "${env.JOB_URL}"
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


