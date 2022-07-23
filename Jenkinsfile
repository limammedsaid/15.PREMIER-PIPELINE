pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *" 
                sh "git clone https://github.com/limammedsaid/15_PREMIER-PIPELINE.git"
            }
        }
        stage('build') { 
            steps {
                sh "cd 15_PREMIER-PIPELINE/ && javac Main.java"
            }
        }
        stage('run') { 
            steps {
                sh " cd 15_PREMIER-PIPELINE && java Main"
            }
        }
    }
}
