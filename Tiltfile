# Deploy: tell Tilt the YAML to deploy
k8s_yaml(helm('chart'))

# Build: Tell Tilt what images to build from which directories
docker_build('dmnkgrc/go-server-test', '.')

# Watch: tell Tilt how to connect locally (optional)
k8s_resource('release-name-go-server-test', port_forwards=8080)
