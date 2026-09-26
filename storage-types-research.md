# Storage Types Research

| Storage Type    | Description                                                                 | Primary Use Case                                      | Cloud Provider Example |
|------------------|------------------------------------------------------------------------------|--------------------------------------------------------|--------------------------|
| Block Storage    | Splits data into fixed-size blocks, each with its own address; behaves like a raw hard drive attached to a server | Databases, OS boot volumes, applications needing low-latency read/write | AWS EBS |
| File Storage     | Organizes data in a hierarchical folder/file structure, accessed over a network via file-sharing protocols | Shared file systems, home directories, content management | AWS EFS |
| Object Storage   | Stores data as discrete objects (data + metadata + unique ID) in a flat address space, accessed via HTTP/API | Unstructured data at scale: images, videos, backups, static web content | AWS S3 |

**Why Object Storage for the client:**
[Write 2-3 sentences here — think about why a photo-sharing app with millions of user uploads needs something that scales horizontally, is accessed over the web via simple API calls, and doesn't require a fixed folder hierarchy the way block or file storage do.]
