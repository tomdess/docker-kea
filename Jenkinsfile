node {
    checkout scm

    docker.image('jonasal/kea-dhcp4:2').withRun('-v $(pwd)/examples/simple:/kea/config', '-c /kea/config/dhcp4.json' ) {
       sh 'make check'
    }
}
