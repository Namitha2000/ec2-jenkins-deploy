pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                echo "Checking out source code"
                git url: 'https://github.com/Namitha2000/ec2-jenkins-deploy.git'
            }
        }


        stage('Deploy Application') {
            steps {
                sh '''
                   sudo cp index.html /var/www/html/index.html
                   sudo systemctl restart apache2
            }
        }
        
    }
