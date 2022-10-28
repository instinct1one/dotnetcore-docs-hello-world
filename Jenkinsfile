<<<<<<< HEAD
pipeline {
    agent {label 'n2'}
    tools {
        dotnetsdk '.net'
    }
    stages {
           stage('CLONE'){
            steps {
                git url:'https://github.com/instinct1one/dotnetcore-docs-hello-world.git', branch :'master'
                 }
                }
        stage('BUILD'){
            steps {
                sh 'dotnet build'
                 }
             }
        stage ('PUBLISH') {
            steps {
                sh 'dotnet publish'
                }
        }
        stage ('ARTIFACTS'){
            steps {
                archiveArtifacts artifacts: '**/*.dll'
                }
             }
    }
=======
pipeline {
    agent {label 'n2'}
    tools {
        dotnetsdk '.net'
    }
    stages {
           stage('CLONE'){
            steps {
                git url:'https://github.com/instinct1one/dotnetcore-docs-hello-world.git', branch :'master'
                 }
                }
        stage('BUILD'){
            steps {
                sh 'dotnet build'
                 }
             }
        stage ('PUBLISH') {
            steps {
                sh 'dotnet publish'
                }
        }
        stage ('ARTIFACTS'){
            steps {
                archiveArtifacts artifacts: '**/*.dll'
                }
             }
    }
>>>>>>> b2140a422e3a5b3c38a77bef0c1de337acf73f64
}