root@DESKTOP-0ANCI6F:~/k8s/k8sCluster_kubeadm_terraform (master)# ssh ubuntu@34.208.103.112
root@ip-172-31-21-83:/etc/kubernetes# ll
total 44
drwxr-xr-x  4 root root 4096 Feb 21 08:49 ./
drwxr-xr-x 95 root root 4096 Feb 21 08:48 ../
-rw-------  1 root root 5644 Feb 21 08:49 admin.conf
-rw-------  1 root root 5676 Feb 21 08:49 controller-manager.conf
-rw-------  1 root root 1968 Feb 21 08:49 kubelet.conf
drwxr-xr-x  2 root root 4096 Feb 21 08:49 manifests/
drwxr-xr-x  3 root root 4096 Feb 21 08:49 pki/
-rw-------  1 root root 5628 Feb 21 08:49 scheduler.conf
root@ip-172-31-21-83:/etc/kubernetes# cd manifests --- pasted the manifest.yaml
root@ip-172-31-21-83:/etc/kubernetes/manifests# vi cloudethix-static.yaml
root@ip-172-31-21-83:/etc/kubernetes/manifests# exit
logout
ubuntu@ip-172-31-21-83:/etc$ exit
logout
Connection to 34.208.103.112 closed.
root@DESKTOP-0ANCI6F:~/k8s/k8sCluster_kubeadm_terraform (master)# kgp
NAME                         READY   STATUS    RESTARTS      AGE
backend-7f5b7998b9-27szm     1/1     Running   0             128m
backend-7f5b7998b9-k9kwf     1/1     Running   0             128m
backend-7f5b7998b9-sddhx     1/1     Running   0             128m
cloudethix-static-master     1/1     Running   0             77s
