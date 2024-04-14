pipeline{
    
    // define agents
    agent any
    

    // define tools
    tools{
        gradle 'gradle'
    }
    

    // define stages
    stages{
        
        // stage 1
        stage("clone git repo"){
            steps{
                git branch: 'master', url:'https://github.com/LukaLmelias/java-todo.git'
            }
        }
        
        
        // stage 2
        stage("Build code"){
            steps{
                sh "gradle build"
            }
        }
        
        // stage 3
        stage("Test"){
            steps{
                sh "gradle test"
            }
            
        }

        
            
        }
    }
}