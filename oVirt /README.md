# oVirt
https://kubevirt.io/2018/Deploying-KubeVirt-on-a-Single-oVirt-VM.html

## packages install
```sh
sudo apt install ansible git wget
```

## ovirt-guest-agent install
```sh
echo 'deb  $REPOURL /' >> /etc/apt/sources.list.d/ovirt-guest-agent.list
wget $REPOURL/Release.key
apt-key add - < Release.key  
sudo apt update
sudo apt install ovirt-guest-agent

sudo systemctl start ovirt-guest-agent
```

## oc install
```sh
wget https://github.com/openshift/origin/releases/download/v3.9.0/openshift-origin-client-tools-v3.9.0-191fece-linux-64bit.tar.gz

tar zxvf openshift-origin-client-tools-v3.9.0-191fece-linux-64bit.tar.gz

cp openshift-origin-client-tools-v3.9.0-191fece-linux-64bit/oc /usr/bin
```

## docker install
省略

```sh
oc cluster up
```