# Monitoring-tools

$ ssh -i ~/Downloads/jenkins.pem ubuntu@35.154.199.152
Welcome to Ubuntu 24.04.2 LTS (GNU/Linux 6.8.0-1029-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/pro

 System information as of Wed Jul  2 07:23:32 UTC 2025

  System load:  0.0                Processes:             115
  Usage of /:   12.6% of 13.49GB   Users logged in:       0
  Memory usage: 5%                 IPv4 address for enX0: 172.31.3.212
  Swap usage:   0%

Expanded Security Maintenance for Applications is not enabled.

0 updates can be applied immediately.

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status


The list of available updates is more than a week old.
To check for new updates run: sudo apt update


The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

ubuntu@ip-172-31-3-212:~$ sudo apt-get update
Hit:1 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble InRelease
Get:2 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates InRelease [126 kB]
Get:3 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports InRelease [126 kB]
Get:4 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/universe amd64 Packages [15.0 MB]
Get:5 http://security.ubuntu.com/ubuntu noble-security InRelease [126 kB]
Get:6 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/universe Translation-en [5982 kB]
Get:7 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/universe amd64 Components [3871 kB]
Get:8 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/universe amd64 c-n-f Metadata [301 kB]
Get:9 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/multiverse amd64 Packages [269 kB]
Get:10 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/multiverse Translation-en [118 kB]
Get:11 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/multiverse amd64 Components [35.0 kB]
Get:12 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/multiverse amd64 c-n-f Metadata [8328 B]
Get:13 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 Packages [1207 kB]
Get:14 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main Translation-en [250 kB]
Get:15 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 Components [161 kB]
Get:16 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/universe amd64 Packages [1098 kB]
Get:17 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/universe Translation-en [279 kB]
Get:18 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/universe amd64 Components [376 kB]
Get:19 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/universe amd64 c-n-f Metadata [26.0 kB]
Get:20 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/restricted amd64 Packages [1367 kB]
Get:21 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/restricted Translation-en [294 kB]
Get:22 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/restricted amd64 Components [212 B]
Get:23 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 Packages [22.1 kB]
Get:24 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/multiverse Translation-en [4972 B]
Get:25 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 Components [940 B]
Get:26 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 c-n-f Metadata [592 B]
Get:27 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/main amd64 Packages [39.2 kB]
Get:28 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/main Translation-en [8676 B]
Get:29 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/main amd64 Components [7080 B]
Get:30 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/main amd64 c-n-f Metadata [272 B]
Get:31 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/universe amd64 Packages [27.1 kB]
Get:32 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/universe Translation-en [16.5 kB]
Get:33 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/universe amd64 Components [16.4 kB]
Get:34 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/universe amd64 c-n-f Metadata [1304 B]
Get:35 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/restricted amd64 Components [216 B]
Get:36 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/restricted amd64 c-n-f Metadata [116 B]
Get:37 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/multiverse amd64 Components [212 B]
Get:38 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-backports/multiverse amd64 c-n-f Metadata [116 B]
Get:39 http://security.ubuntu.com/ubuntu noble-security/main amd64 Packages [958 kB]
Get:40 http://security.ubuntu.com/ubuntu noble-security/main Translation-en [172 kB]
Get:41 http://security.ubuntu.com/ubuntu noble-security/main amd64 Components [21.5 kB]
Get:42 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Packages [865 kB]
Get:43 http://security.ubuntu.com/ubuntu noble-security/universe Translation-en [189 kB]
Get:44 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Components [52.2 kB]
Get:45 http://security.ubuntu.com/ubuntu noble-security/universe amd64 c-n-f Metadata [17.0 kB]
Get:46 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 Packages [1322 kB]
Get:47 http://security.ubuntu.com/ubuntu noble-security/restricted Translation-en [285 kB]
Get:48 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 Components [208 B]
Get:49 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 Packages [17.7 kB]
Get:50 http://security.ubuntu.com/ubuntu noble-security/multiverse Translation-en [3792 B]
Get:51 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 Components [208 B]
Get:52 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 c-n-f Metadata [380 B]
Fetched 35.1 MB in 17s (2026 kB/s)
Reading package lists... Done
ubuntu@ip-172-31-3-212:~$ sudo apt-get install -y docker.io
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  bridge-utils containerd dns-root-data dnsmasq-base pigz runc ubuntu-fan
Suggested packages:
  ifupdown aufs-tools cgroupfs-mount | cgroup-lite debootstrap docker-buildx docker-compose-v2
  docker-doc rinse zfs-fuse | zfsutils
The following NEW packages will be installed:
  bridge-utils containerd dns-root-data dnsmasq-base docker.io pigz runc ubuntu-fan
0 upgraded, 8 newly installed, 0 to remove and 33 not upgraded.
Need to get 79.2 MB of archives.
After this operation, 300 MB of additional disk space will be used.
Get:1 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/universe amd64 pigz amd64 2.8-1 [65.6 kB]
Get:2 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/main amd64 bridge-utils amd64 1.7.1-1ubuntu2 [33.9 kB]
Get:3 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 runc amd64 1.2.5-0ubuntu1~24.04.1 [8043 kB]
Get:4 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 containerd amd64 1.7.27-0ubuntu1~24.04.1 [37.7 MB]
Get:5 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/main amd64 dns-root-data all 2024071801~ubuntu0.24.04.1 [5918 B]
Get:6 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/main amd64 dnsmasq-base amd64 2.90-2build2 [375 kB]
Get:7 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble-updates/universe amd64 docker.io amd64 27.5.1-0ubuntu3~24.04.2 [33.0 MB]
Get:8 http://ap-south-1.ec2.archive.ubuntu.com/ubuntu noble/universe amd64 ubuntu-fan all 0.12.16 [35.2 kB]
Fetched 79.2 MB in 1s (91.0 MB/s)
Preconfiguring packages ...
Selecting previously unselected package pigz.
(Reading database ... 70681 files and directories currently installed.)
Preparing to unpack .../0-pigz_2.8-1_amd64.deb ...
Unpacking pigz (2.8-1) ...
Selecting previously unselected package bridge-utils.
Preparing to unpack .../1-bridge-utils_1.7.1-1ubuntu2_amd64.deb ...
Unpacking bridge-utils (1.7.1-1ubuntu2) ...
Selecting previously unselected package runc.
Preparing to unpack .../2-runc_1.2.5-0ubuntu1~24.04.1_amd64.deb ...
Unpacking runc (1.2.5-0ubuntu1~24.04.1) ...
Selecting previously unselected package containerd.
Preparing to unpack .../3-containerd_1.7.27-0ubuntu1~24.04.1_amd64.deb ...
Unpacking containerd (1.7.27-0ubuntu1~24.04.1) ...
Selecting previously unselected package dns-root-data.
Preparing to unpack .../4-dns-root-data_2024071801~ubuntu0.24.04.1_all.deb ...
Unpacking dns-root-data (2024071801~ubuntu0.24.04.1) ...
Selecting previously unselected package dnsmasq-base.
Preparing to unpack .../5-dnsmasq-base_2.90-2build2_amd64.deb ...
Unpacking dnsmasq-base (2.90-2build2) ...
Selecting previously unselected package docker.io.
Preparing to unpack .../6-docker.io_27.5.1-0ubuntu3~24.04.2_amd64.deb ...
Unpacking docker.io (27.5.1-0ubuntu3~24.04.2) ...
Selecting previously unselected package ubuntu-fan.
Preparing to unpack .../7-ubuntu-fan_0.12.16_all.deb ...
Unpacking ubuntu-fan (0.12.16) ...
Setting up dnsmasq-base (2.90-2build2) ...
Setting up runc (1.2.5-0ubuntu1~24.04.1) ...
Setting up dns-root-data (2024071801~ubuntu0.24.04.1) ...
Setting up bridge-utils (1.7.1-1ubuntu2) ...
Setting up pigz (2.8-1) ...
Setting up containerd (1.7.27-0ubuntu1~24.04.1) ...
Created symlink /etc/systemd/system/multi-user.target.wants/containerd.service → /usr/lib/systemd/system/containerd.service.
Setting up ubuntu-fan (0.12.16) ...
Created symlink /etc/systemd/system/multi-user.target.wants/ubuntu-fan.service → /usr/lib/systemd/system/ubuntu-fan.service.
Setting up docker.io (27.5.1-0ubuntu3~24.04.2) ...
info: Selecting GID from range 100 to 999 ...
info: Adding group `docker' (GID 113) ...
Created symlink /etc/systemd/system/multi-user.target.wants/docker.service → /usr/lib/systemd/system/docker.service.
Created symlink /etc/systemd/system/sockets.target.wants/docker.socket → /usr/lib/systemd/system/docker.socket.
Processing triggers for dbus (1.14.10-4ubuntu4.1) ...
Processing triggers for man-db (2.12.0-4build2) ...
Scanning processes...
Scanning linux images...

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
ubuntu@ip-172-31-3-212:~$ sudo usermod -aG docker ${USER}
ubuntu@ip-172-31-3-212:~$ newgrp docker
ubuntu@ip-172-31-3-212:~$ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
ubuntu@ip-172-31-3-212:~$ newgrp docker
ubuntu@ip-172-31-3-212:~$ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
ubuntu@ip-172-31-3-212:~$ sudo usermod -aG docker ${USER}
ubuntu@ip-172-31-3-212:~$ newgrp docker
ubuntu@ip-172-31-3-212:~$ docker ls
docker: 'ls' is not a docker command.
See 'docker --help'
ubuntu@ip-172-31-3-212:~$ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
ubuntu@ip-172-31-3-212:~$ git clone https://github.com/KiranPolaki/docker-voting-app
cd docker-voting-app
Cloning into 'docker-voting-app'...
remote: Enumerating objects: 88, done.
remote: Counting objects: 100% (88/88), done.
remote: Compressing objects: 100% (71/71), done.
remote: Total 88 (delta 14), reused 82 (delta 10), pack-reused 0 (from 0)
Receiving objects: 100% (88/88), 2.04 MiB | 6.74 MiB/s, done.
Resolving deltas: 100% (14/14), done.
ubuntu@ip-172-31-3-212:~/docker-voting-app$ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
ubuntu@ip-172-31-3-212:~/docker-voting-app$ chmod +x kind-cluster/install-kind.sh
chmod +x kind-cluster/install-kubectl.sh
chmod: cannot access 'kind-cluster/install-kind.sh': No such file or directory
chmod: cannot access 'kind-cluster/install-kubectl.sh': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ls
LICENSE      architecture.excalidraw.png  docker-stack.yml  k8s-specifications  seed-data
MAINTAINERS  docker-compose.images.yml    healthchecks      kind-cluster        vote
README.md    docker-compose.yml           image.png         result              worker
ubuntu@ip-172-31-3-212:~/docker-voting-app$ chmod +x kind-cluster/install_kind.sh
chmod +x kind-cluster/install_kubectl.sh
ubuntu@ip-172-31-3-212:~/docker-voting-app$ chmod +x kind-cluster/install-kind.sh
chmod: cannot access 'kind-cluster/install-kind.sh': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ^C
ubuntu@ip-172-31-3-212:~/docker-voting-app$ chmod +x install-kind.sh
chmod +x install-kubectl.sh
chmod: cannot access 'install-kind.sh': No such file or directory
chmod: cannot access 'install-kubectl.sh': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app$ chmod +x kind-cluster/install-kind.sh
chmod +x kind-cluster/install-kubectl.sh
chmod: cannot access 'kind-cluster/install-kind.sh': No such file or directory
chmod: cannot access 'kind-cluster/install-kubectl.sh': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app$ chmod +x/install-kind.sh
chmod: missing operand after ‘+x/install-kind.sh’
Try 'chmod --help' for more information.
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ^[[200~chmod +x kind-cluster/install-kind.sh
chmod: command not found
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ~chmod +x kind-cluster/install-kind.sh
Command '~chmod' not found, did you mean:
  command 'chmod' from deb coreutils (9.4-2ubuntu2)
Try: sudo apt install <deb name>
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ps
    PID TTY          TIME CMD
   1252 pts/0    00:00:00 bash
   2345 pts/0    00:00:00 bash
   2359 pts/0    00:00:00 bash
   2379 pts/0    00:00:00 bash
   2466 pts/0    00:00:00 ps
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ls
LICENSE      architecture.excalidraw.png  docker-stack.yml  k8s-specifications  seed-data
MAINTAINERS  docker-compose.images.yml    healthchecks      kind-cluster        vote
README.md    docker-compose.yml           image.png         result              worker
ubuntu@ip-172-31-3-212:~/docker-voting-app$ cd kind-cluster
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ ls kind-cluster
ls: cannot access 'kind-cluster': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ ls kind-cluster/
ls: cannot access 'kind-cluster/': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ chmod +x install-kind.sh
chmod +x install-kubectl.sh
chmod: cannot access 'install-kind.sh': No such file or directory
chmod: cannot access 'install-kubectl.sh': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ chmod +x kind-cluster/install-kind.sh
chmod +x kind-cluster/install-kubectl.sh
chmod: cannot access 'kind-cluster/install-kind.sh': No such file or directory
chmod: cannot access 'kind-cluster/install-kubectl.sh': No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ cd ..
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ./kind-cluster/install_kind.sh
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    97  100    97    0     0    397      0 --:--:-- --:--:-- --:--:--   399
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100 6304k  100 6304k    0     0  3826k      0  0:00:01  0:00:01 --:--:-- 62.5M
ubuntu@ip-172-31-3-212:~/docker-voting-app$ ./kind-cluster/install_kubectl.sh
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   138  100   138    0     0    459      0 --:--:-- --:--:-- --:--:--   461
100 49.0M  100 49.0M    0     0  35.9M      0  0:00:01  0:00:01 --:--:-- 56.0M
Client Version: v1.30.0
Kustomize Version: v5.0.4-0.20230601165947-6ce0bf390ce3
kubectl installation complete.
ubuntu@ip-172-31-3-212:~/docker-voting-app$ cd kind-cluster
kind create cluster --config=config.yml --name=my-cluster
Creating cluster "my-cluster" ...
 ✓ Ensuring node image (kindest/node:v1.30.0) 🖼
 ✓ Preparing nodes 📦 📦 📦
 ✓ Writing configuration 📜
 ✓ Starting control-plane 🕹️
 ✓ Installing CNI 🔌
 ✓ Installing StorageClass 💾
 ✓ Joining worker nodes 🚜
Set kubectl context to "kind-my-cluster"
You can now use your cluster with:

kubectl cluster-info --context kind-my-cluster

Thanks for using kind! 😊
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ kubectl get nodes
NAME                       STATUS   ROLES           AGE   VERSION
my-cluster-control-plane   Ready    control-plane   35s   v1.30.0
my-cluster-worker          Ready    <none>          12s   v1.30.0
my-cluster-worker2         Ready    <none>          14s   v1.30.0
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ ls
commands.md  config.yml  dashboard-adminuser.yml  install_kind.sh  install_kubectl.sh
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ cd k8s-specifications/
bash: cd: k8s-specifications/: No such file or directory
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ cd ..
ubuntu@ip-172-31-3-212:~/docker-voting-app$ cd k8s-specifications/
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ kubectl apply -f
error: flag needs an argument: 'f' in -f
See 'kubectl apply --help' for usage.
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ kubectl apply -f .
deployment.apps/db created
service/db created
deployment.apps/redis created
service/redis created
deployment.apps/result created
service/result created
deployment.apps/vote created
service/vote created
deployment.apps/worker created
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ kubectl get all
NAME                          READY   STATUS              RESTARTS   AGE
pod/db-597b4ff8d7-tlvr2       1/1     Running             0          18s
pod/redis-796dc594bb-dq7s2    1/1     Running             0          18s
pod/result-d8c4c69b8-5rjx8    1/1     Running             0          18s
pod/vote-69cb46f6fb-n2c7t     0/1     ContainerCreating   0          18s
pod/worker-5dd767667f-fx947   0/1     ContainerCreating   0          18s

NAME                 TYPE        CLUSTER-IP      EXTERNAL-IP   PORT(S)          AGE
service/db           ClusterIP   10.96.182.185   <none>        5432/TCP         18s
service/kubernetes   ClusterIP   10.96.0.1       <none>        443/TCP          4m24s
service/redis        ClusterIP   10.96.254.151   <none>        6379/TCP         18s
service/result       NodePort    10.96.152.165   <none>        5001:31001/TCP   18s
service/vote         NodePort    10.96.100.243   <none>        5000:31002/TCP   18s

NAME                     READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/db       1/1     1            1           18s
deployment.apps/redis    1/1     1            1           18s
deployment.apps/result   1/1     1            1           18s
deployment.apps/vote     0/1     1            0           18s
deployment.apps/worker   0/1     1            0           18s

NAME                                DESIRED   CURRENT   READY   AGE
replicaset.apps/db-597b4ff8d7       1         1         1       18s
replicaset.apps/redis-796dc594bb    1         1         1       18s
replicaset.apps/result-d8c4c69b8    1         1         1       18s
replicaset.apps/vote-69cb46f6fb     1         1         0       18s
replicaset.apps/worker-5dd767667f   1         1         0       18s
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ kubectl get all nodes
error: you must specify only one resource
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ kubectl get all node
error: you must specify only one resource
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ kubectl get node
NAME                       STATUS   ROLES           AGE     VERSION
my-cluster-control-plane   Ready    control-plane   5m21s   v1.30.0
my-cluster-worker          Ready    <none>          4m58s   v1.30.0
my-cluster-worker2         Ready    <none>          5m      v1.30.0
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ kubectl get all
NAME                          READY   STATUS    RESTARTS   AGE
pod/db-597b4ff8d7-tlvr2       1/1     Running   0          83s
pod/redis-796dc594bb-dq7s2    1/1     Running   0          83s
pod/result-d8c4c69b8-5rjx8    1/1     Running   0          83s
pod/vote-69cb46f6fb-n2c7t     1/1     Running   0          83s
pod/worker-5dd767667f-fx947   1/1     Running   0          83s

NAME                 TYPE        CLUSTER-IP      EXTERNAL-IP   PORT(S)          AGE
service/db           ClusterIP   10.96.182.185   <none>        5432/TCP         83s
service/kubernetes   ClusterIP   10.96.0.1       <none>        443/TCP          5m29s
service/redis        ClusterIP   10.96.254.151   <none>        6379/TCP         83s
service/result       NodePort    10.96.152.165   <none>        5001:31001/TCP   83s
service/vote         NodePort    10.96.100.243   <none>        5000:31002/TCP   83s

NAME                     READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/db       1/1     1            1           83s
deployment.apps/redis    1/1     1            1           83s
deployment.apps/result   1/1     1            1           83s
deployment.apps/vote     1/1     1            1           83s
deployment.apps/worker   1/1     1            1           83s

NAME                                DESIRED   CURRENT   READY   AGE
replicaset.apps/db-597b4ff8d7       1         1         1       83s
replicaset.apps/redis-796dc594bb    1         1         1       83s
replicaset.apps/result-d8c4c69b8    1         1         1       83s
replicaset.apps/vote-69cb46f6fb     1         1         1       83s
replicaset.apps/worker-5dd767667f   1         1         1       83s
ubuntu@ip-172-31-3-212:~/docker-voting-app/k8s-specifications$ cd ../kind-cluster/
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
Downloading https://get.helm.sh/helm-v3.18.3-linux-amd64.tar.gz
Verifying checksum... Done.
Preparing to install helm into /usr/local/bin
helm installed into /usr/local/bin/helm
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ helm --versiom
Error: unknown flag: --versiom
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ helm --version
Error: unknown flag: --version
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ helm version
version.BuildInfo{Version:"v3.18.3", GitCommit:"6838ebcf265a3842d1433956e8a622e3290cf324", GitTreeState:"clean", GoVersion:"go1.24.4"}
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ kubectl create namespace monitoring
namespace/monitoring created
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo add stable https://charts.helm.sh/stable
helm repo list
helm repo update
"prometheus-community" has been added to your repositories
"stable" has been added to your repositories
NAME                    URL
prometheus-community    https://prometheus-community.github.io/helm-charts
stable                  https://charts.helm.sh/stable
Hang tight while we grab the latest from your chart repositories...
...Successfully got an update from the "prometheus-community" chart repository
...Successfully got an update from the "stable" chart repository
Update Complete. ⎈Happy Helming!⎈
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ kubectl create namespace monitoring      Error from server (AlreadyExists): namespaces "monitoring" already exists
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ helm install kind-prometheus prometheus-community/kube-prometheus-stack --namespace monitoring --set prometheus.service.type=NodePort --set prometheus.service.nodePort=30000 --set grafana.service.type=NodePort --set grafana.service.nodePort=31000 --set alertmanager.service.type=NodePort --set alertmanager.service.nodePort=32000
NAME: kind-prometheus
LAST DEPLOYED: Wed Jul  2 07:56:25 2025
NAMESPACE: monitoring
STATUS: deployed
REVISION: 1
NOTES:
kube-prometheus-stack has been installed. Check its status by running:
  kubectl --namespace monitoring get pods -l "release=kind-prometheus"

Get Grafana 'admin' user password by running:

  kubectl --namespace monitoring get secrets kind-prometheus-grafana -o jsonpath="{.data.admin-password}" | base64 -d ; echo

Access Grafana local instance:

  export POD_NAME=$(kubectl --namespace monitoring get pod -l "app.kubernetes.io/name=grafana,app.kubernetes.io/instance=kind-prometheus" -oname)
  kubectl --namespace monitoring port-forward $POD_NAME 3000

Visit https://github.com/prometheus-operator/kube-prometheus for instructions on how to create & configure Alertmanager and Prometheus instances using the Operator.
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ kubectl get pods -n monitoring
NAME                                                     READY   STATUS    RESTARTS   AGE
alertmanager-kind-prometheus-kube-prome-alertmanager-0   2/2     Running   0          114s
kind-prometheus-grafana-7565dc9bdf-26k6t                 3/3     Running   0          2m3s
kind-prometheus-kube-prome-operator-df978f4df-f9qck      1/1     Running   0          2m3s
kind-prometheus-kube-state-metrics-698d8db8c5-fzmtx      1/1     Running   0          2m3s
kind-prometheus-prometheus-node-exporter-bwrzp           1/1     Running   0          2m3s
kind-prometheus-prometheus-node-exporter-djph5           1/1     Running   0          2m3s
kind-prometheus-prometheus-node-exporter-hsg6h           1/1     Running   0          2m3s
prometheus-kind-prometheus-kube-prome-prometheus-0       2/2     Running   0          114s
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ kubectl port-forward svc/kind-prometheus-kube-prome-prometheus -n monitoring 9090:9090 --address 0.0.0.0 &
[1] 10071
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ Forwarding from 0.0.0.0:9090 -> 9090
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
E0702 08:10:44.935976   10071 portforward.go:398] error copying from local connection to remote stream: writeto tcp4 172.31.3.212:9090->14.98.177.234:34084: read tcp4 172.31.3.212:9090->14.98.177.234:34084: read: connection reset by peer
E0702 08:10:44.936276   10071 portforward.go:398] error copying from local connection to remote stream: writeto tcp4 172.31.3.212:9090->14.98.177.234:34072: read tcp4 172.31.3.212:9090->14.98.177.234:34072: read: connection reset by peer
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
Handling connection for 9090
^C
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ kubectl port-forward -n monitoring svc/kind-prometheus-grafana 3000:80 --address 0.0.0.0 &
[2] 10751
ubuntu@ip-172-31-3-212:~/docker-voting-app/kind-cluster$ Forwarding from 0.0.0.0:3000 -> 3000
Handling connection for 9090
Handling connection for 9090
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 9090
Handling connection for 9090
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 3000
Handling connection for 9090
Handling connection for 3000

Broadcast message from root@ip-172-31-3-212 (Wed 2025-07-02 09:13:16 UTC):

The system will power off now!

Connection to 35.154.199.152 closed by remote host.
Connection to 35.154.199.152 closed.
