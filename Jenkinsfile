pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'echo "Fallo!"; exit 1'
            }
        }
    }
    post {
        always {
            echo 'Siempre se ejecuta'
        }
        success {
            echo 'Ejecucion exitosa'
        }
        failure {
            echo 'Fallo en la ejecucion'
        }
        unstable {
            echo 'Ejecucion inestable'
        }
        changed {
            echo 'La Pipeline ha cambiado'
            echo 'Por ejemplo, Si estaba fallando pero ahora es exitosa'
        }
    }
}
