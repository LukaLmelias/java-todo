pipeline{
    agent any
    
    tools{
        gradle 'gradle'
    }
    
    stages{
        
        
        stage("clone git repo"){
            steps{
                git branch: 'master', url:'https://github.com/LukaLmelias/java-todo.git'
            }
        }
        
        
        
        stage("Build code"){
            steps{
                sh "gradle build"
            }
        }
        
        stage("Test"){
            steps{
                sh "gradle test"
            }
        }
    }
}