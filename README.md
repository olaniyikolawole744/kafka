# kafka
This project creates kafka nodes with topic, a producer that write to the topic and consumer reading from the topic.
run the packer modules with packer build
run the terraform vpc module with terraform init, terraform plan and terraform apply
copy the ansible inventory and playbook into the .ansible/tmp folder
run the ansible playbook with Ansible-playbook playbook/playbookbroker.yml -i inventory/hosts/host
start the zookeeper with bin/zookeeper-server-start.sh config/zookeeper.properties
start the kafka broker with bin/kafka-server-start.sh config/server.properties
run the producer with python producer_message.py
run the consumer with python consumer_message.py
