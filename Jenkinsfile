pipeline {
    agent any
    parameters {
        string(name: 'yyyyy', defaultValue: 'XXX', description: 'Hello world')

        text(name: 'Demo', defaultValue: '', description: 'Demo parameter')

        booleanParam(name: 'Boolean', defaultValue: true, description: 'Boolean value')

        choice(name: 'CHOICE', choices: ['A', 'B', 'C'], description: ‘Choose one')

        password(name: 'PASSWORD', defaultValue: 'Key', description: 'Enter a password')

        file(name: "FILE", description: "file to upload")
    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.yyyyy}"

                echo "Biography: ${params.Demo}"

                echo "Toggle: ${params.Boolean }"

                echo "Choice: ${params.CHOICE}"

                echo "Password: ${params.PASSWORD}"
            }
        }
    }
}
