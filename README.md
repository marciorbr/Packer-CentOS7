# Criando Template CentOS 7 com Packer VMware Builder

Este repositório contém Templates packer para build de Template Linux no VMware vSphere.

 

# Utilização:

1. Renomeei o arquivo example-variables.json e insira o valores de seu ambiente.

2. Valide o código.

```command
$ packer validate -var-file=variables.json CentOS7.json
Template validated successfully.
```

3. Por fim faça o Build.

```command
packer build -var-file=variables.json CentOS7.json
```

# Arquivos utilizados:

* JetBrains-infra vSphere-iso (File Name: packer-builder-vsphere-iso.macos)  https://github.com/jetbrains-infra/packer-builder-vsphere

* Packer  https://www.packer.io

* CentOS 7.x ISO  https://wiki.centos.org/Download - use a ISO DVD.
