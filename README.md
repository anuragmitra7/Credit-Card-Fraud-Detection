ML-Gitops
![ML Gitops](https://user-images.githubusercontent.com/92513084/161149928-72159a41-92d7-4202-8cf1-e695810a6004.gif)
Overview ✍️
In this project we craeted a SBI-Loan-Status Ml-Flask App, This App simply check the loan status of a customer [Code] [Demo].
We write the Dockerfile to create the Docker Image of SBI-Loan-Status and push that local repository to central repository(Guthub), using Github Action we create docker image of SBI-Loan-Status and push on the docker hub repository [Code] [Demo] .
And using Helm chart we Launch pods on kubernetes of SBI-Loan-Status image. If any changes happen in Ml-Flask App Github Action Automatically trigger and create the new image of changes code with same name and different tag and push on dockerHub. In Helm chart just we updated image tag name in value.yaml file, kubernetes Launch new pods of new image and terminating the old pods without any downtime using rolling update strategy.

Goal 🎯
To achieve Automation 🤖 in Data Science Project.

Step To Involve Create This Project 👣

1.Created Ml-Flask App.
Demo
Link:- https://loan-status-app.herokuapp.com/
