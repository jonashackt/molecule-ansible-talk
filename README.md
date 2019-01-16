# molecule-ansible-talk

### Test-driven infrastructure development

```
molecule create --scenario-name vagrant-ubuntu
molecule verify --scenario-name vagrant-ubuntu
molecule converge --scenario-name vagrant-ubuntu
molecule verify --scenario-name vagrant-ubuntu
molecule destroy --scenario-name vagrant-ubuntu
```


### Continuous infrastructure TravisCI

[TravisCI build](https://travis-ci.org/jonashackt/molecule-ansible-docker-vagrant/builds/472056229?utm_source=github_status&utm_medium=notification)


### Continuous Cloud infrastructure TravisCI + AWS

https://eu-central-1.console.aws.amazon.com/ec2/v2/home?region=eu-central-1

```
molecule create --scenario-name aws-ec2-ubuntu
molecule converge --scenario-name aws-ec2-ubuntu
molecule verify --scenario-name aws-ec2-ubuntu
molecule destroy --scenario-name aws-ec2-ubuntu
```