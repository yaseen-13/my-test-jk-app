
node{
    def mavenHome = tool name: 'maven3.9.8'
    stage('1CloneCode'){
    //    git "https://github.com/nfestaclass04/maven-web-application.git"
        git branch: 'main', url: 'https://github.com/yaseen-13/my-test-jk-app.git'
    }
    /*
    stage('2Test&Build'){
        sh "${mavenHome}/bin/mvn clean install"
   }
   
   stage('3UploadArtifacts'){
        sh "${mavenHome}/bin/mvn deploy"
    }
 
    stage('7DeploymentToProd'){
        deploy adapters: [tomcat9(credentialsId: 'tomcat-cred', path: '', url: 'http://18.118.84.108:8080/')], contextPath: null, war: 'target/*war'
    }
    */
}

   
