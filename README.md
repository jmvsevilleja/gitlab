# Gitlab in Container

Gitlab Runner in Container

docker run -d --name gitlab-runner -v /var/run/docker.sock:/var/run/docker.sock -v /srv/{runner-name}/config:/etc/gitlab-runner --rm gitlab/gitlab-runner 

docker exec -it gitlab-runner gitlab-runner register -n --url http://192.168.80.166 --registration-token qWxSUQU6Huy2LYzHKSKP --clone-url http://192.168.80.166 --executor docker --docker-image "docker:latest" --docker-privileged 

OR https://gist.github.com/SolidNerd/1bf47f85457e4f90eea541586f7290da
