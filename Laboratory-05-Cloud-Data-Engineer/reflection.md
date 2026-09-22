# Mission Reflection

This laboratory helped me understand why object storage is useful for
applications that need to store a very large number of files such as
photos. Object storage is designed for unstructured data and organizes
objects inside buckets. Compared with traditional block storage, it is
more suitable for applications that need to store large collections of
images because files can be managed as objects together with their
associated metadata.

Docker made deploying the MinIO storage server easier because I did not
need to manually install and configure every component of the storage
software. The Docker command downloaded the MinIO image and started the
server with the required ports and environment variables. This made the
deployment process faster and more consistent.

A bucket is a logical container used to organize objects in object
storage. In this activity, I created a bucket named `client-photos`.
The bucket provided a location where the sample image or text file could
be uploaded and managed.

Large enterprise companies can use several techniques to reduce the risk
of losing object storage data when physical hardware fails. These can
include keeping multiple copies of data, using redundancy, replicating
data across storage systems or locations, and maintaining backups.
These approaches help make data available even when individual hardware
components experience problems.

My confidence in navigating the Linux command line has also improved.
At the beginning, commands such as `docker run` and `docker ps` were
unfamiliar, but I became more comfortable entering commands and checking
their output. I learned that command-line skills are important for cloud
engineering because many cloud services and containers can be deployed
and managed through terminal commands. This activity also helped me
understand how Docker, MinIO, ports, buckets, and object storage work
together as part of a cloud environment.
