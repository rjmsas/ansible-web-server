pipeline{
    agent{
        label "ansibleworker1"
    }
    stages{
        stage("install-httpd"){
            steps{
                sh '''
                ansible-playbook -i host nginx-ansible.yml
                '''
            }
        }
    }
}