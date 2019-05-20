### Creating new services/applications
These instructions are written assuming we are spinning up instances at AWS.  Once we migrate our work over to the Pathology infrastructure, these instructions will need updating

#### Spin up new service at AWS
1) Log into http://aws.it.umich.edu/ with your level 1 credentials
2) Click on EC2
3) Click Launch Instance
4) Search for "ami-0ac019f4fcb7cb7e6"
5) Click Community AMIs
6) Click Select on "ubuntu/images/hvm-ssd/ubuntu-bionic-18.04-amd64-server-20180912 "
7) Determine what size machine you will need and select appropriately
8) Click "Next: Configure Instance Details"
- Select the following options:
Network: "vpc-0b06f40f50a5ce1e2"
Subnet: "subnet-0e8645e44813a14d3"
Enable termination protection: Check the box

9) Click "Next: Add Storage"
- Determine if you need any additional storage added to this instance and configure it here

10) Click "Next: Add tags"
- Add a tag called "Name" with a name that looks like "`<service name> - <instance type>`", where instance type is DEV, QA or PROD.  For example: Demo - DEV

11) Click "Next: Configure Security Group"
- Select "Select an existing security group"
- Select "UMDefaultWEBGroup" and "UMDefaultWEBGroup"

12) Click "Review and Launch"
- Review the details to ensure everything looks right.
- If anything is wrong you can click on the links at the top to return to the section that has an issue and fix it

13) Click "Launch"
- Choose "Choose an existing key pair"
- For select a key pair, select "um-kpmp"
- Check the "acknowledge" checkbox


#### Associate IP addresses with the new instances
1) From the Service dropdown at the top (or the side panel) Select Elastic IPs
2) Allocate new addresses if there are no unallocated ones you can use
- click allocate new address
- select Amazon Pool
- Click allocate
- Click close

3) Associate address with instance
- Select the new ip address
- Click "Actions"
- Select "Associate Address"
- Type the name in "instance" and select the appropriate instance
- Click "Associate"

#### Getting domain names registered, ssl certs and shib certs
1) email jprosser@uw.edu
2) give him the domain names we selected and the associated ip addresses
