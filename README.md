# vagrant-docker-jenkins

Based on **Ubuntu 18.04 LTS** box.
Jenkins hosted on port **8080** with *smartbear:password* credentials.
Tested only with virtualbox provider so please run with "*vagrant up --provider virtualbox*"
Both Jenkins and scheduler that runs cron to create new jobs every 5 minutes are dockerized
For Jenkins bitnami/jenkins image was used. Scheduler is based on openjdk:slim
