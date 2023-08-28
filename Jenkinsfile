pipeline {
    agent any
    stages {
        stage('Ejemplo') {
            input {
                message "Ingresa tu edad"
                ok "Siguiente"
                submitter "alice,bob"
                parameters {
                    string(nombre: 'NOMBRE', defaultValue: 'JENKINS', description: 'Cual es tu nombre?')
                    String(edad: 'EDAD', descriptions: 'Ingresa tu edad')
                }
            }
            steps {
                echo "Hola, ${NOMBRE}, mucho gusto conocerte."
                echo " tienes ${EDAD} años."
            }
        }
    }
}
