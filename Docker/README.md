![jng4w](../img/jng4w.jpg)

#Docker (v.20.10.14)

##Installation

### Step 1

Run command below in CMD:
```
sudo yum remove docker \
                  docker-client \
                  docker-client-latest \
                  docker-common \
                  docker-latest \
                  docker-latest-logrotate \
                  docker-logrotate \
                  docker-engine
```
### Step 2
Run command below in CMD:
```
sudo yum install -y yum-utils
```
### Step 3
Run command below in CMD:
```
sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo
```
### Step 4
Run command below in CMD:
```
sudo yum install docker-ce-20.10.14 docker-ce-cli-20.10.14 containerd.io docker-compose-plugin
```
If false, then install additional packages below first:
```
sudo yum install http://mirror.centos.org/centos/7/extras/x86_64/Packages/container-selinux-2.107-1.el7_6.noarch.rpm
```
```
sudo yum install http://mirror.centos.org/centos/7/extras/x86_64/Packages/slirp4netns-0.4.3-4.el7_8.x86_64.rpm
```
### Step 5
Add script below to to file `/etc/yum.repos.d/docker-ce.repo` (using `sudo nano docker-ce.repo`):

```
[centos-extras]
name=Centos extras - $basearch
baseurl=http://mirror.centos.org/centos/7/extras/x86_64
enabled=1
gpgcheck=1
gpgkey=http://centos.org/keys/RPM-GPG-KEY-CentOS-7
```

### Step 6

```
sudo yum -y install fuse-overlayfs
```

## Verification

* Start docker: 

    ```
    sudo systemctl start docker
    ```

* Verify that Docker Engine is installed correctly by running the hello-world image: 

    ```
    sudo docker run hello-world
    ```
