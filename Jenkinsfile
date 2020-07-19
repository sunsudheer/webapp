pipeline {
    agent {}
    stages {
/*
        stage('Clone') { 
            steps {
                git url:'https://github.com/veer-c/git_lab.git', branch: 'master'
            }
        }
*/
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean install' 
            }
        }
    }
   post {
        always {
            echo 'I am Mr Always'
        }
        success {
            echo 'I succeeeded!'
        }
    }
}

