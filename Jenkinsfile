pipeline {
    agent any
    tools{
        maven 'mvn'
        jdk 'jdk'
    }
    stages {
        stage('code'){
            steps{
                echo'coding'
        }
    }
    stage('build'){
        steps{
            echo'building'
            sh 'mvn clean package -DskipTests'
            sh 'mvn install'
        }
    }
    
    stage('test'){
        steps{
            echo 'for testing'
            sh 'mvn test'
            sh 'mvn install'
        }
    }
    
    stage('deploy'){
        steps{
            echo'deploying'
        }
    }
    
}
}
