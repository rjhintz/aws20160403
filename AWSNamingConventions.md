## Naming Conventions
### Instances
Note: Auto scaling creates names. Use a Tag for your own naming.

Tag values are case-sensitive and accept a maximum of 255 Unicode [characters](http://docs.aws.amazon.com/cli/latest/reference/ec2/run-instances.html)
### S3
> calculate a short hash (note: collisions don’t matter here, just pseudo-randomness) and 
> pre-pend it to the string you wish to use for your object name. 
> This way, operations are again fanned out over multiple partitions. To list keys with common prefixes, 
> several list operations can be performed in parallel, one for each unique character prefix in your hash.

### Security Groups
Name constraints:
* Up to 255 characters in length
* for EC2-VPC: a-z, A-Z, 0-9, spaces, and `._-:/()#,@[]+=;{}!$*`

### Key Pairs
Name constraint: Up to 255 ASCII characters

### References
#### Create [Run] Instance
[CLI Run Instance](http://docs.aws.amazon.com/cli/latest/reference/ec2/run-instances.html)
#### Key Pair
[CLI create key pair](http://docs.aws.amazon.com/cli/latest/reference/ec2/create-key-pair.html)
#### Security Group
[CLI create security group](http://docs.aws.amazon.com/cli/latest/reference/ec2/create-security-group.html)
#### S3
[Amazon S3 Performance Tips & Tricks](https://aws.amazon.com/blogs/aws/amazon-s3-performance-tips-tricks-seattle-hiring-event/)

#### Naming Convention Guidance From Others
> Naming Conventions: AWS assets should be named in such a way they can be readily identified, 
> a suggested standardization around the purpose of the Instance, its environment, its region, and its sequence number.  
> An example of this might be `haddop_dn_prod_usw1_001`, this represents a production Hadoop data node, in the US-West 1 region.

> a. When naming an AMI its a good practice to include the creation date as part of its name, and a complete description. 
>This will minimize confusion when selecting ami for new instances.

> b. When naming security groups and key pairs, continue to use the convention purpose, environment, region, function.  
> For example `db_prod_usw1_key` or `ws_prod_usw1_sg`

(http://www.xervmon.com/amazon-aws-best-practices-enterprise-perspective/)

[AWS Tips I Wish I'd Known Before I Started](https://wblinks.com/notes/aws-tips-i-wish-id-known-before-i-started/)
