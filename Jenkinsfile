node{
    
    stage('GIT'){
        git 'https://github.com/SarfrazPNQ/game-of-life.git'
    }
    
    stage('Build & package'){
        sh label: '', script: 'mvn package'
    }
    
    stage('Artifactory'){
        archiveArtifacts 'gameoflife-web/target/gameoflife.war'
    }
	}