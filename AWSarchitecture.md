## AWS Architecture

### Resources
*  [AWS re:Invent 2015 | (ARC301) Scaling Up to Your First 10 Million Users - video](https://youtu.be/vg5onp8TU6Q)
*  [AWS re:Invent 2014 | (SPOT301) AWS Innovation at Scale - James Hamilton video](https://youtu.be/JIQETrFC_SQ)
*  [Deep Dive: Scaling Up to Your First 10 Million Users - video](https://youtu.be/KulMgJnMLsw)
  *  14:55 Start with SQL
  *  29:14
    *  move static context from web instance to S3 / Cloudfront
    *  move session state and database caching to Elasticache / DynamoDB
    *  move dynamic content from ELB balancer to Cloudfront
*  [AWS re:Invent 2015 | (ARC403) From One to Many: Evolving VPC Design - video](https://youtu.be/ykmqjgLdmL4)
*  [AWS re:Invent 2015 | (NET403) Another Day, Another Billion Packets- video](https://youtu.be/3qln2u1Vr2E)
    
