pipeline {
    agent any

    stages {
        stage('compile code') {
            steps {
                //sh 'echo static content'
                echo 'Hello World'
            }
        }
        stage('test') {
            steps {
                // sh 'echo static content'
                echo 'Hello World'
            }
        }
        stage('code quality') {
            steps {
                // sh 'sonar qube command'
                echo 'Hello World'
            }
        }
        stage('code security') {
            when {
                expression { env.BRANCH_NAME == "main" }
            }
            steps {
                echo 'we go there'
            }
        }
        stage('Release') {
            when {
                expression { env.TAG_NAME ==~ ".*" }
            }
            steps {
                echo 'Hello World'
            }
        }
    }
}