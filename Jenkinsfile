node {

    checkout scm

    docker.withRegistry('cloudzune/hello-kaniko', 'docker') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
