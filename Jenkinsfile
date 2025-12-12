pipeline {
    agent any
    environment{
        INSTAGRAM_X="@Xpiritu"
    }
    stages{
        stage("Saludo 1"){
            steps{
                echo "Hola desde Saludo 1"
            }
        }
        stage("Saludo 2"){
            steps{
                echo "Hola desde Saludo 2, paso 1"
                echo "Hola desde Saludo 2, paso 2"
            }
        }
        stage("Imprimir variable de entorno"){
            steps{
                echo "${env.INSTAGRAM_X}"
                echo "${INSTAGRAM_X}"
                echo "$INSTAGRAM_X"
                echo "============================"
                sh "echo ${env.INSTAGRAM_X}"
                sh "echo ${INSTAGRAM_X}"
                sh "echo $INSTAGRAM_X"
            }
        }
        stage("Imprimir variable de entorno, definida en System"){
            steps{
                echo "${env.INSTAGRAM}"
                echo "${INSTAGRAM}"
                echo "$INSTAGRAM"
                echo "==========================="
                sh "echo ${env.INSTAGRAM}"
                sh "echo ${INSTAGRAM}"
                sh "echo $INSTAGRAM"
                sh """echo $INSTAGRAM"""
            }
        }
    }
}
