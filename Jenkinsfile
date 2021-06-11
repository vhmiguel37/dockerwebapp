node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'docker-miguelv') {

        def customImage = docker.build("040500/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}