pipeline{
        agent any
        environment {
            PYTHON= 'C:\\Users\\priya\\AppData\\Local\\Programs\\Python\\Python313\\python.exe'
        }
        trigger{
            cron("*/2 * *  * *")
        }
        stages{
            stage('checkout code'){
                steps{

                checkout scm

                }
            }
            stage("extract data"){
                steps{
                bat "${env.PYTHON} extractdata.py"
                }

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