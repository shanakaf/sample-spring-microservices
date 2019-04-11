
node {
    stage('Checkout') {
        git branch: 'develop', credentialsId: 'githubId', url: 'https://github.com/shanakaf/sample-spring-microservices'
    }

    stage('Build') {
        def mvnHome = tool name: 'maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn clean install"
    }     
}