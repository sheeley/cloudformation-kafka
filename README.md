# Overview 
Cloudformation template for Kafka, leveraging Exhibitor's Cluster endpoint to find zookeeper hosts.

## Usage
1. Create VPC & Subnets 
2. Set up zookeeper & exhibitor. I suggest using https://github.com/sheeley/cloudformation-zookeeper
3. Create cloudformation stack using `kafka.json` and enter `http://your-exhibitor-loadbalanacer-domain` with no trailing slash in the `ExhibitorLoadBalancer` field.

## TODO
- [ ] When Kafka-Manager supports it, automatically set the cluster of kafka brokers.
- [ ] Return URL(s) for Kafka-Manager instances.
