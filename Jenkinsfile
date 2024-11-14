pipeline{
    agent { label 'test-node' } 
    tools{
        maven "maven3.9.8"
    }
    stages{
        stage('1CodeClone'){
            steps{
                sh "echo 'This is the latest version of Tesla application.'"
                git branch: 'main', url: 'https://github.com/yaseen-13/my-test-jk-app.git'
            }
        }
        stage('2Test&Build'){
            steps{
                sh "echo 'Maven should be able to do a build now'"
                sh "mvn clean install"
            }
        }
        /*
        stage('4UploadArtifacts'){
            steps{
                sh "echo 'pushing Artifacts to remote repository'"
                sh "mvn deploy"
            }
        }
        stage('5DeploymentToUat'){
            steps{
                sh "echo 'Deployment to Tomcat'"
                deploy adapters: [tomcat9(credentialsId: 'tomcat-cred', path: '', url: 'http://3.128.25.158:8080/')], contextPath: null, war: 'target/*war' 
            }
        }
        */
    }
}


   
