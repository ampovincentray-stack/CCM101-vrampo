# Mission Reflection

The lab has given me insight into the advantages of object storage for the storage of large amounts of data like images. Object storage is developed and constructed to deal with unstructured data, storing various objects in buckets. This storage system is different from conventional block storage as it is better suited for applications involving the mass storage of images due to its ability to handle files along with their relevant metadata together with them.

Using Docker simplified the process of deploying MinIO storage server because I have not had to install and configure all its parts manually. With the help of Docker command, MinIO image was downloaded and server was started with the needed ports and environment variables. This approach has sped up the process of deployment.

Buckets serve as sensible containers that help with classifying the objects in object storage. In this case, I prepared a bucket called client-photos. The bucket served as a location where a sample image jpg can be uploaded and handled.

Big businesses are able to apply various methods to minimize the chances of losing stored information caused by hardware breakdowns. These include storing multiple copies of information, introducing redundancy, replicating data over different storage systems or places, and taking backups of information. The mentioned practices guarantee that the data is accessible in the event of a malfunction of equipment.

I have gained more confidence in utilizing the Linux command line as well. At first, I didn’t understand what “docker run” and “docker ps” meant, but I managed to make use of the command line. I came to the realization that it is very important for a cloud engineer to have information about the command line since a number of cloud technologies and containers are operated via commands in the command line interface. Besides, I learned how such concepts as Docker, MinIO, ports, buckets, and object storage work in the cloud during this experience.
