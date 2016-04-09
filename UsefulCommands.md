Look in `~/bin`




```
aws ec2 describe-vpcs --vpc-ids vpc-8a495fee --output table
---------------------------------------------------------------------------------------------------
|                                          DescribeVpcs                                           |
+-------------------------------------------------------------------------------------------------+
||                                             Vpcs                                              ||
|+---------------+----------------+------------------+------------+-------------+----------------+|
||   CidrBlock   | DhcpOptionsId  | InstanceTenancy  | IsDefault  |    State    |     VpcId      ||
|+---------------+----------------+------------------+------------+-------------+----------------+|
||  172.16.0.0/16|  dopt-37ca3052 |  default         |  False     |  available  |  vpc-8a495fee  ||
|+---------------+----------------+------------------+------------+-------------+----------------+|
```

`aws ec2 describe-subnets --filters Name=vpc-id,Values=vpc-8a495fee --output table`



```
aws ec2 describe-availability-zones --output text
AVAILABILITYZONES	us-east-1	available	us-east-1a
AVAILABILITYZONES	us-east-1	available	us-east-1b
AVAILABILITYZONES	us-east-1	available	us-east-1c
AVAILABILITYZONES	us-east-1	available	us-east-1d
AVAILABILITYZONES	us-east-1	available	us-east-1e
```



```
#!/bin/bash
# Put in ˜/bin - Needs chmod 755 <filename>
# Execute: ./hello_world
echo 'Hello World!' #another comment
#
#  a=z                   # Assign the string "z" to variable a
#  b="a string"         # Embedded spaces must be within quotes.
#  c="a string and $b"  # Other expansions such as variables can be expanded into the assignment.
#  d=$(ls -l foo.txt)   # Results of a command.
#  e=$((5 * 7))         # Arithmetic expansion.
#  f="\t\ta string\n"   # Escape sequences such as tabs and newlines.
```
