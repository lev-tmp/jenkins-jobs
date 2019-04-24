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