stage('parallel') {
        def stages = [:]

        stages["Node1"] = {
            node(label:'trey') {
                sh 'echo $NODE_NAME'
            }
        }
        stages["Node2"] = {
            node(label:'fakenodelabelhere') {
                sh 'echo $NODE_NAME'
            }
        }

        parallel(stages)
}
