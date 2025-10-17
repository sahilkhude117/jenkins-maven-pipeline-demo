new item -> pipeline -> git with scm

# install jdk
    - enter to jenkis shel -> sudo docker exec -u root -it jenkins-container bash
    - apt update -y
    - apt install -y wget apt-transport-https gnupg
    - wget -O- https://packages.adoptium.net/artifactory/api/gpg/key/public | gpg --dearmor -o /usr/share/keyrings/adoptium-archive-keyring.gpg
    - echo "deb [signed-by=/usr/share/keyrings/adoptium-archive-keyring.gpg] https://packages.adoptium.net/artifactory/deb bookworm main" > /etc/apt/sources.list.d/adoptium.list
    - apt update -y
    - apt install -y temurin-17-jdk
    - java -version



