pipeline {
    agent any
    environment {
        gitURL  =   "https://github.com/AltheaOlofsson/TrailrunnerJenkins.git"
    }
    parameters {
        choice choices: ['main', 'B1'], description: "Choose which branch to run", name: "Branch"
    }

    stages {
        stage('Checkout') {
            steps {
                script {
                    git branch: params.Branch, url: "${gitURL}"
                }
            }
        }
        stage('Clean Maven') {
            steps {
                echo 'Stage 2'
            }
        }
        stage('Build Trailrunner') {
            steps {
                echo 'Stage 3'
            }
        }
        stage('Test trailrunner') {
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