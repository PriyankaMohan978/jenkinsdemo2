node{
    try{
    stage('checkout code'){
        checkout scm

    }
    stage('extract data'){
        
        bat 'C:\\Users\\priya\\AppData\\Local\\Programs\\Python\\Python313\\python.exe'
    }
    }
    catch(err){

        echo "pipeline error: ${err}"

    }
    finally {
        echo "pipeline completed"
    }
}
