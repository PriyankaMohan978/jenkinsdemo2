pipeline{
        agent any
        environment {
            PYTHON= 'C:\\Users\\priya\\AppData\\Local\\Programs\\Python\\Python313\\python.exe
'
        }
        stages{
            stage('checkout code'){
                checkout scm

            }
            stage("extract data"){
                bat "${env.PYTHON} extract.py"


            }
        }
        post {

            success{
                echo "success...."


            }
            failure{
                echo "failure....."

            }
            always{
                echo "always....."


            }
        }




}