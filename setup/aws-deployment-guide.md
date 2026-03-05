# AWS Deployment Guide

## Launch EC2 Instance

Instance type: t3.micro  
Operating System: Ubuntu 22.04  
Storage: 8GB

Security Group Rules:

SSH (22) – My IP  
HTTP (80) – My IP

## Install Docker

sudo apt update
sudo apt install docker.io -y

## Run OWASP Juice Shop

sudo docker run -d -p 80:3000 bkimminich/juice-shop

## Access Application

http://<EC2-Public-IP>
