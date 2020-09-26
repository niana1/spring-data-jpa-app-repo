pipeline {
    agent any
    stages{
        stage('Maven compile'){
            steps{
                echo 'Project compile stage'
                bat label: 'compilation running',script:'''mvn compile'''
            }
        }
        stage('Unit test'){
            steps{
                echo 'Project Testing stage'
                bat label: 'test running', script: '''mvn test'''
            }
        }
        stage('maven package'){
            steps{
                echo 'Project packaging stage'
                bat label: 'project packaging', script: '''mvn package'''
            }
        }
    }
}