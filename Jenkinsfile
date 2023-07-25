pipeline {
    agent any
    stages {
        stage('stage-1') {
            steps {
                echo "stage-1 boshlandi.."
                sh '''
                echo "starting stage-1 process again..."
                '''
            }
        }
        stage('stage-2') {
            steps {
                echo "stage-2 boshlandi.."
                sh '''
                echo "starting stage-2 process again..."
                '''
            }
        }
        stage('stage-3-updated....') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "starting delivery process..."
                '''
            }
        }
    }
}
