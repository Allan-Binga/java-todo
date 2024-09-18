pipeline{
    agent any
    tools{
        gradle "Gradle-6"
    }
    stages{
        stage ('Cloning Repository') {
            steps{
                git branch:'master', url: 'https://github.com/Allan-Binga/java-todo'
            }
        }
        stage ('Build project') {
            steps{
                sh 'gradle build'
            }
        }
        stage ('Tests') {
            steps {
                sh 'gradle test'
            }
        }
    
}