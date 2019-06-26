pipeline {
    agent any
    stages {

        stage('apache install'){
          steps{
		    echo 'installing apache from Jenkins through Git'
                //sh 'mkdir from-jenkins'
                //sh 'touch from-jenkins/test.txt'
		    echo 'running palybook' 
                sh '''
                   ansible-playbook -i hosts -s -u ubuntu apache.yml 
                '''
                }
        }

}
}
