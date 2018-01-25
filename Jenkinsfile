node {
   stage('Code Preparation') { 
     git credentialsId: 'GithubID', url: 'https://github.com/galaxyset/new-venture.git'
   }
   stage('Compile & Build') {
     withMaven(jdk: 'JDK1.8', maven: 'Maven-3.5.2') {
       sh 'mvn clean compile'
     }
   }
   stage('Test') {
      echo 'Test executed'
   }
   stage('Results') {
       echo 'Results are generated'
   }
   stage('Artifactory') {
       echo 'Archived Reports to Artifactory'
   }
   stage('Deploy to Dev') {
       echo 'Deployed the Dev'
   }
   stage('Deploy to QA') {
       echo 'Deployed the QA'
   }
}
