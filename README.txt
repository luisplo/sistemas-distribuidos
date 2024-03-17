# Construir proyecto

```bash
docker-compose up -d --build 
```

# Enviar archivo desde el cliente al servidor

```bash
docker-compose exec nfsv4-client bash -c "echo 'Hello NFS' > /nfs_mount/test.txt"
```

# Verificar si existe el archivo en el servidor

```bash
docker-compose exec nfsv4-server cat /nfs_share/test.txt
```