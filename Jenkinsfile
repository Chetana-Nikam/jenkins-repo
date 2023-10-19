pipeline {
    agent { node { label 'built-in' } }

    stages {
        stage ('Hello') {

            steps {
                
                    echo 'Hello !!!'
                }
            
        }

        stage ('Good Bye') {

            steps {
                
                    echo 'Good Bye !!!'
                }
            
        }
        
        stage ('Echo Branch') {

            steps {
                
                    echo "This is master branch"
                }
            
        }
    }
}
