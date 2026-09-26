# MinIO Deployment Documentation

## Docker Command Used

docker run -d -p 9000:9000 -p 9001:9001 --name minio-server
-e "MINIO_ROOT_USER=cloudadmin"
-e "MINIO_ROOT_PASSWORD=CloudNova2026!"
minio/minio server /data --console-address ":9001"


## Access Details
- **Web Console Port:** 9001
- **API Port:** 9000
- **Bucket Created:** client-photos

## Environment Variables Explained
The `-e` flags pass environment variables into the container at startup, letting you configure it without editing files inside the image:
- `MINIO_ROOT_USER=cloudadmin` — sets the admin username for the MinIO server.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` — sets the admin password for the MinIO server.

Both credentials are used to log into the MinIO web console at port 9001.
