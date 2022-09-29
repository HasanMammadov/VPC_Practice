# VPC

To achive isolated network.

## Description

Using Bastion Host we gonna creat connection between public and private subnets.

### Create below atributes in AWS.

* 1.  VPC in AWS.
* 2.  Subnets.
* 3.  Route Tables
* 4.  Internet Gateway
* 5. NACL's
* 6. NAT Gateway
*  Also we need creat 2 EC2. 1st for Bastion host, 2nd for private subnets.

### Assosation Subnets.

* After creating public and private subnets we need assosiate subnets.
* For high availability creat subnets in different AZ's.
### Internet Gateway.

* 1 VPC can have 1 Intenet Gateway. 
* Attach VPC to Gateway.

### Route Tables.

* We need creat public and private RT. 
* We need configure inbound rukles and outband rules. 

### NACL's (A Network Access Control List).

* We need 3 NACL
1. Bustion
2. Public
3. Private 
* Inbound rules:
  Add rule number (110), Custop TCP, Port - 22 for SSH, and destination local IP. 
* Outband rules:
  Add rule number (110), Custop TCP, Port - 1024 -65535, and destination local IP. 

### Creat Security Groups.

* We need 3 NACL.
1. Bustion
2. Public
3. Private 
* Inbound rules:
  Add rule number (110), Custop TCP, Port - 22 for SSH, and destination local IP. 
* Outband rules:
  Add rule number (110), Custop TCP, Port - 1024 -65535, and destination local IP. 
## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

 Hasan Mammadov  
[@HasanMammad](https://www.linkedin.com/in/hasan-mamedoff-073a30212/)

## Version History

* 0.1
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.2
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)