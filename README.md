# CI Project

## Dev 
> PEQUERY Gregory

> PORQUET Antoine

> LEBEAU Mike

## Global goal

Push on `git` -> start `Jenkins` -> if `success` -> merge on `master` -> push on `Nexus`


## Dev part

Part wich contains the maven project

## Docker part 

Part wich contains the dockers

Docker GitLab -> Greg

Docker Jenkins -> Mike

Docker SonarQube -> Antoine

Docker Nexus -> Mike

## Tips

### Share containers althrough several computers

After running your container and mapping his ports, you have to 
set the forwarding ports 

> in VirtualBox : Configuration -> Network(NAT) -> Advanced
-> add your IP address

Then on your firewall settings : 

> On Windows : Add new inbound rules (use a port between 5000 and 5010 to avoid ESGI's blocked ports)