properties([parameters([choice(choices: ['master', 'hello-world-1', 'hello-world-2'], description: 'Select branch to build', name: 'branch')])])

node {

    stage ('SCM Checkout') {

        echo 'Pulling change from the branch ${params.branch}'
        git url: 'https://github.com/ysyzdykov/mp2019_codeRepo.git', branch '${params.branch}'

    }

    stage ('Print a message') {

        echo 'Hello world!'

    }

}
