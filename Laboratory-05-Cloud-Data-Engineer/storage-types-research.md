# Storage Types Research

## Comparison Table

| Storage Type   | Description | Primary Use Case | Cloud Provider Example |
|----------------|--------------------------------------------------------------------------------------------|------------------------------------------------------------------|--------------------------|
| Block Storage  | Splits data into fixed-size blocks, each with its own address, and presents itself like a raw disk attached directly to a server or VM. | Databases, operating system boot volumes, and applications that need fast, low-latency read/write access. | AWS EBS |
| File Storage   | Organizes data in a traditional hierarchical folder/file structure, accessed over a shared network using protocols like NFS or SMB. | Shared file systems, content management systems, and applications needing simultaneous access from multiple servers. | AWS EFS |
| Object Storage | Stores data as individual objects (the data itself, metadata, and a unique identifier) inside a flat, non-hierarchical namespace, accessed through HTTP-based APIs. | Storing massive amounts of unstructured data such as images, videos, documents, and backups at scale. | AWS S3 |

## Why Object Storage is Best for Client Photos

For a photo-sharing application storing millions of user-uploaded images, Object Storage is the clear choice because it can scale almost limitlessly without being tied to a single server's physical disk, unlike Block Storage. It is also accessed directly through simple web (HTTP) requests, which fits naturally into a modern web application's architecture. Finally, each object carries useful metadata and a unique key, making it easier and cheaper to organize, retrieve, and serve large volumes of images reliably.
