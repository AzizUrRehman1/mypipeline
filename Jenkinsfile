node {

    checkout scm

    docker.withRegistry('https://hub.docker.com/', 'docker-q321') {

        def customImage = docker.build("q321/mypipeline")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
