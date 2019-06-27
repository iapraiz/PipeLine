pipeline{
    agent { label 'windows' }
    triggers {
      cron '* * * * *'
    }    
    stages{
        stage('Saludo'){
            steps{
                echo 'Hola'
            }
        }
        stage('Version'){
            steps{
                echo 'Version de Maven'
            }
        }          
        stage('Despedida'){
            steps{
                echo 'Adios'
            }
        }        
    }
    post{
        always{
            echo 'PD: sALGO SIEMPRE'
        }
        success{
            echo 'Acabo sin problemas'
        }
        changed{
            echo 'Esto ha cambiado'
        }                
        failure{
            echo 'Error'
        }
        regression{
            echo 'Antes iba y ahora no'
        }
    }
}
