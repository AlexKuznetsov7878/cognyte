pipeline {
    agent any

    stages {
        stage('Clean repo'){
            steps {
                sh 'rm -rf ./*'
            }
        }
        stage('Clone repo') {
            steps {
                sh "git clone https://github.com/AlexKuznetsov7878/cognyte.git"
            }
        }
        stage('Run code'){
            steps {
                sh 'pwd'
                sh 'echo CHECK'
                sh 'chmod 777 /var/jenkins_home/workspace/pipeline_job/cognyte/example.sh'
                sh '/var/jenkins_home/workspace/pipeline_job/cognyte/example.sh'
                sh 'chmod 777 /var/jenkins_home/workspace/pipeline_job/cognyte/example.py'
                sh 'python3 /var/jenkins_home/workspace/pipeline_job/cognyte/example.py'
            }
        }
    }
}
