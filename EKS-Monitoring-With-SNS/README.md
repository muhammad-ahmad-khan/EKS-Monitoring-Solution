# EKS Monitoring With SNS  

Setup Prometheus (Operator) and Grafana monitoring on an AWS EKS cluster with Alertmanager notifications via Amazon SNS.  

## Description  

This project provides a comprehensive monitoring solution for Amazon EKS using the `kube-prometheus-stack`, which includes Prometheus, Grafana, and Alertmanager. It also covers configuring an ALB Ingress for external access and setting up Amazon SNS as the Alertmanager receiver.  

Using SNS as a receiver simplifies email notifications without requiring an SMTP setup. Instead, multiple email addresses can be subscribed to the SNS topic for alert distribution. However, note that SNS has limitations, such as not rendering HTML content correctly—alerts will be received as plain text instead of formatted HTML.

## Dependencies  

* Helm  
* Kubectl  
* AWS CLI or AWS Console access  
* AWS Load Balancer Controller must be installed in the EKS cluster  

### How to execute the solution?

* See the write up [here.](https://dev.to/muhammad_ahmad_khan/monitoring-alerting-for-aws-eks-using-grafana-prometheus-alertmanager-with-sns-integration-5593)

