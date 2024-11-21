@Library('kobalty-jenkins-shared@main') _
import com.moandjiezana.toml.Toml

pipeline {
    agent any
    stages {
        stage("Load pipeline configuration") {
            steps {
                echo '${env}'
                script {
                    def toml = new Toml()
                    echo "Git repo URL: ${config.git.url}"
                }
            }
        }
        stage('Build') {
            steps {
                // Build steps (e.g., compile code, run unit tests)
                echo "Building..."
                echo "Finished building."
            }
        }
        stage('Test') {
            steps {
                // Test steps (e.g., run integration tests)
                echo "Running unit tests..."
                echo "Results: " 
                echo "Running integration tests" 
                echo "Results: " 
            }
        }
        stage('Deploy') {
            steps {
                // Deployment steps (e.g., deploy to staging/production)
                echo "Deploying application..."
                echo "Finished deploying."
            }
        }
    }
}