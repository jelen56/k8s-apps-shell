# k8s-apps-shell
#### This is a script repository related to k8s common services/apps deployment, use, and configuration, such as `postgresql`, `cri-dockerd`,developed by using shell scripts

### the apps support list:
- `postgresql`
- `cri-dockerd`
- ...(coming soon)

### usage:
- `postgresql`:
  - `init`: `bash pgsql-install.sh init`
  - `reset`: `bash pgsql-install.sh reset`
  - **NOTE**:`reset` means deleting the related datas and resource(such as services),Generally used when you want to reinstall `postgresql`;btw,`pgsql-install.sh` is developed based on `local Persistent Volumes`,The config selection combination of volumes is [`configMap`](https://kubernetes.io/docs/concepts/storage/volumes/#configmap),[`local Persistent Volumes`](https://kubernetes.io/docs/concepts/storage/volumes/#local)

- `cri-dockerd`:
  - `init`:`bash cri-dockerd-install.sh init`
  - `reset`:`bash cri-dockerd-install.sh reset`,**NOTE**:`reset` means deleting the related datas and resource(such as services),Generally used when you want to reinstall postgresql

  
