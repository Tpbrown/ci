==== To create a ci machine in ec2 ====

* cp secrets_template.yml secrets.yml
* Fill out secrets.yml
* install vagrant version 1.7.4+
* vagrant plugin install vagrant-aws
* install ansible "brew install ansible" for mac
* vagrant up --provider=aws
* add cloud foundry credentials as environment variables in the gocd pipeline:
  * CF_EMAIL: <your cloud foundry login>
  * CF_PASSWORD: <your cloud foundry password>

