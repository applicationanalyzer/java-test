pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            label 'slave04'
        }
    }
stages
{
  stage('clone') {
            steps
            {
              git 'https://github.com/TejaswiniTharigopula2295/java-working.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
}
}
