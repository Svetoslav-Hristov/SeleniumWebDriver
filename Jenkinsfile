pipeline{
    agent any
    
    
    stages{
        stage("Restore dependencies"){
            steps{
                bat 'dotnet restore'
            }
            
        }
        
         stage("Build Solution"){
            steps{
                bat 'dotnet build'
            }
            
        }
         stage("Run Tests"){
            steps{
                echo "Running Tests 1"
                bat 'dotnet test TestProject1 '
                echo "Running Tests 2"
                bat 'dotnet test TestProject2 '
                echo "Running Tests 3"
                bat 'dotnet test TestProject3 ' 
            }
            
            
        }


    }
    
}