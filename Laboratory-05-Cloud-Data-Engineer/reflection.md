# Mission Reflection

This laboratory gave me a better understanding of how object storage can be used in cloud applications. Storing millions of photos using object storage is more suitable because photos are unstructured files and each one can be stored as an individual object. Instead of depending on the storage of one traditional computer, an object storage system is designed to manage large collections of files and make them available to applications.

Docker also made the MinIO deployment easier. Instead of installing the storage server manually and configuring many components separately, I could start MinIO through a Docker command. The command also allowed me to specify the ports and administrator credentials before starting the container.

A bucket is a container used to organize objects in an object storage system. In this activity, I created the `client-photos` bucket and used it to store a sample uploaded file. Seeing the file inside the bucket made the concept of object storage easier to understand because I was able to interact with the storage service through its web interface.

Large organizations need to protect their stored information from hardware failures. They can use backups, replication, multiple storage devices, and copies of information in different locations. These methods can help an organization recover data if a physical machine or storage device becomes unavailable.

I also became more comfortable with the Linux command line during this activity. I used commands to work with my GitHub repository, create folders, start a Docker container, and check the container status. At first, the commands required more attention because a small mistake could prevent a service from starting. After checking the results of each command, I became more comfortable using the terminal. This activity also showed me how command-line tools and web interfaces can work together when managing a cloud service.
