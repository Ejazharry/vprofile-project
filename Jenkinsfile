pipeline {
    agent any
    tools {
        maven "MAVEN3"
        jdk "OracleJDK8"
    }

   environment {
        SNAP_REPO = 'vprofile-snapshot'
		NEXUS_USER = 'admin'
		NEXUS_PASS = 'Ishan9739'
		RELEASE_REPO = 'vprofile-release'
		CENTRAL_REPO = 'vprofile-maven-central'
		NEXUSIP = '13.40.103.6'
		NEXUSPORT = '8081'
		NEXUS_GRP_REPO = 'vprofile-maven-group'
        NEXUS_LOGIN = 'nexuslogin'
    }

    stages {
        stage ('Build'){
            steps {
                sh 'mvn install -y'
            }
        }
    }
}