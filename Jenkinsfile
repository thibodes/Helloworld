pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Hier klonen we de broncode van het Git-repository
                git 'https://github.com/thibodes/helloworld'
            }
        }
        stage('Build') {
            steps {
                // Hier voeren we een eenvoudige buildstap uit
                sh 'javac Helloworld.java'
            }
        }
        stage('Test') {
            steps {
                // Hier kunnen testen worden uitgevoerd, indien beschikbaar
                // Voor dit eenvoudige voorbeeld slaan we dit over
            }
        }
        stage('Run') {
            steps {
                // Hier voeren we de applicatie uit
                sh 'java Helloworld'
            }
        }
    }
}
