pipeline {
    agent { 
        node { 
            label 'built-in' 
            customWorkspace '/home/ec2-user' 
        } 
    }
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }

    stages {
        stage ('Hello') {

            steps {
                
                    echo 'Hello !!!'
                
                    sh 'touch 11.txt'
                    sh 'pwd'
                    echo 'Your previous buid no is: ${BUILD_NUMBER}'
                    echo 'Your previous buid no is: ${BUILD_NUMBER}'
                    echo 'Your jenkins home is: ${JENKINS_HOME}'
                    echo "Hello ${params.PERSON}"
    
                    echo "Biography: ${params.BIOGRAPHY}"
    
                    echo "Toggle: ${params.TOGGLE}"
    
                    echo "Choice: ${params.CHOICE}"
    
                    echo "Password: ${params.PASSWORD}"
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
