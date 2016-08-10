# packer_itamae

## Description
You could make AMI constructed rails environment. 
Inside this packer Itamae runs to install ruby and rails as provisioner.


## Requirement

- packer 0.10.x


## Usuage

In variables.json file, you have to set your aws access key and secret key.
```
vi variables.json
```

You could validate your template.
```
packer validate -var-file=variables.json template.json
```

Run packer to make AMI.
```
packer build -var-file=variables.json template.json
```