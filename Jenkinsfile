node {

    stage('Clone Repository') {
        git branch: 'main', url: 'https://github.com/Akshaya7032/MavenProject2.git'
    }

    stage('Clean') {
        bat "mvn clean -f pom.xml"
    }

    stage('Build') {
        bat "mvn install -f pom.xml"
    }

    stage('Test') {
        bat "mvn test -f pom.xml"
    }

    stage('Package') {
        bat "mvn package -f pom.xml"
    }
}
