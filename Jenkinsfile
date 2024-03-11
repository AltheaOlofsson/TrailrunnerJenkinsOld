pipeline {
    agent any
    stages {
        stage('Stage1') {
            steps {
                echo 'Stage 1'
            }
        }
        stage('Stage2') {
            steps {
                echo 'Stage 2'
            }
        }
        stage('Stage3') {
            steps {
                echo 'Stage 3'
            }
        }
        stage('Stage4') {
            steps {
                echo 'Stage 4'
            }
            post { 
                always { 
                    echo 'stage 4.5!'
                }
            }
        }
        
    }
}