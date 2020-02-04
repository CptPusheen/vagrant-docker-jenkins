# vagrant-docker-jenkins

Based on **Ubuntu 18.04 LTS** box.
Jenkins hosted on port **8080**. To login use:<details><summary>click to reveal</summary>smartbear:password credentials</details>
Tested only with virtualbox provider so please run with "*vagrant up --provider virtualbox*"
Both Jenkins and scheduler that runs cron to create new jobs every 5 minutes are dockerized.
For Jenkins **bitnami/jenkins** image was used, scheduler is based on **openjdk:slim**
