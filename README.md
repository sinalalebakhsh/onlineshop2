# onlineshop2


## run on ubuntu

    If you want to use server ubuntu:
    Installing Docker:
    sudo apt update
    sudo apt install apt-transport-https ca-certificates curl software-properties-common
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
    sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
    apt-cache policy docker-ce
        Output of apt-cache policy docker-ce
            docker-ce:
            Installed: (none)
            Candidate: 5:19.03.9~3-0~ubuntu-focal
            Version table:
                5:19.03.9~3-0~ubuntu-focal 500
                    500 https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
    sudo apt install docker-ce
    sudo systemctl status docker

    Installing Docker Compose:
    sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    sudo chmod +x /usr/local/bin/docker-compose
    docker-compose --version
        Output
        docker-compose version 1.29.2, build 5becea4c
        
    docker-compose up --build

