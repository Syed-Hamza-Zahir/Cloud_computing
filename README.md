 # Cloud_computing
![Computer-Networks-Cloud-Computing-Diagrams-Cloud-Computing-Types.png](./Computer-Networks-Cloud-Computing-Diagrams-Cloud-Computing-Types.png)

## Public Cloud 

• A service provider makes resources, such as virtual machines (VMs), applications or storage, available to the general public over the Internet 

• Public cloud services may be free or offered on a pay-per-usage model 

• The main difference between public and private clouds is that the individual or organization is not responsible for any of the management of a public cloud hosting solution 

• The data is stored in the provider's data center and the provider is responsible for the management and maintenance of the data center

# Private Cloud 

• A private cloud is a cloud computing model that involves a secure cloud based environment where only the specified organization can access its resources 

• Data center may be wholly in-house on the company’s premises, or provided by a third party 

• Private cloud services can vary considerably from a technical aspect, therefore it is usually categorized by the features that they offer to their client

# Hybrid 

• Hybrid cloud is a cloud computing environment which uses a mix of on-premises, private cloud, and third-party, public cloud services with adaptation between the two platforms 

• By allowing loads to move between private and public clouds as computing needs change, the hybrid cloud gives organizations greater flexibility and data deployment options

# Relationship between Local and Cloud Resources 

• The traditional IT model advantages and disadvantages 
  
  - Advantages: Very secure/full control of applications and data 
  
  - Disadvantages: Own Hardware/upgrades, software/upgrades, power/issues, redundancy and business continuity, large in-house IT department 

• Cloud computing model advantages and disadvantages 

  - Advantages: Flexibility and scalability with hardware, software, power issues, redundancy and business continuity are handled by vendor, and smaller IT department 
  
  - Disadvantages: Security might be a primary concern, expertise with application needs

## AWS

AWS stands for Amazon Web Services to contrast their shipping services. It is a collection of services that Amazon provides online. These are things like storage, backup, DNS, database, load balancing and maybe the most popular, virtual machine hosting. The concept about all this is the economy of scale. Amazon will build huge data centers and engineer them to provide the kind of services that most businesses need. Since they do it on a huge scale they are able to do it cheaper then if every business were to build their own from scratch. There are however lots of disadvantages like needing a lot more spare capacity and having to build something that fits everyone as opposed to something that fits a particular user. So it depends on the use case if you save money by using their services as opposed to making your own from scratch.

One of the most revolutionary benefits that AWS brought into the market is that purchasing additional capacity is much easier and faster. You might have taken weeks to buy hardware and install it at your location. Or if you are renting though traditional suppliers you might take a few hours to let them manually reconfigure things. However AWS made everything automatic so you can get a new server within seconds. This have allowed businesses to build their applications to allow them to scale on demand. This means that they pay different amount of money for the services depending on how much they use. This have the ability to reduce costs but it again require more time to develop and maintain the more complex applications.

## AWS Services
![aws-perspective-architecture-diagram.9cc2f8ed5212705854c027f54bcc00221112db2c.png](./aws-perspective-architecture-diagram.9cc2f8ed5212705854c027f54bcc00221112db2c.png)

# Connect to Your Linux Instance using an SSH Client
- ``ssh -i /path/my-key-pair.pem ec2-user@ec2-198-51-100-1.compute-1.amazonaws.com``
- (``ssh -i /path/my-key-pair.pem user@ip_address`` )

# Copying Files Between Local Computer and Instance (AWS)
- To copy files between your computer and your instance you can use an FTP service like FileZilla or the command scp which stands for secure copy.
- To use scp with a key pair use the following command: ``scp -i path/to/key file/to/copy user@ip_address:path/to/file.``
- To use it without a key pair, just omit the flag -i and type in the password of the user when prompted.
- To copy an entire directory, add the -r recursive option:
``scp -i path/to/key -r directory/to/copy user@ip_address:path/to/directory``

# Deployment
- Use SSH Agent plugin
  - Add credentials - SSH username with private key
  - Add the .pem private key created in AWS
- Execute shell

# Connect to Your Linux Instance using an SSH Client
- ``ssh -i /path/my-key-pair.pem user@ip_address`` 

# Copying Files Between Local Computer and Instance (AWS)
- To copy files between your computer and your instance you can use an FTP service like FileZilla or the command scp which stands for secure copy.
- To use scp with a key pair use the following command: ``scp -i path/to/key file/to/copy user@ip_address:path/to/file.``
- To use it without a key pair, just omit the flag -i and type in the password of the user when prompted.
- To copy an entire directory, add the -r recursive option:
``scp -i path/to/key -r directory/to/copy user@ip_address:path/to/directory``
