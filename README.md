puppetmaster clients for orawls,oradb modules
=============================================

use puppet client 3.4.3 works together with my vagrant-puppetmaster github repos

- vagrant up oradb (oracle database 11.2.0.4 )
- vagrant up adminwls with nodewls1 & nodewls2 (cluster 10.3.6)
- vagrant up adminwls2 ( adminserver 10.3.6 )
- vagrant up adminwls3 ( adminserver 12.1.2 )
- vagrant up adminwls4 ( adminserver + osb PS6 + soa suite PS6 ( with bpm & bam ))
- vagrant up adminwls5 ( adminserver + osb PS6 )

vagrant ssh xxx

su -
use vagrant as password

service iptables stop
echo "10.10.10.2 puppet.grahamgilbert.dev puppet"  >> /etc/hosts

cd /etc/puppet/
vi puppet.conf

add server to the main section
[main]
   server = puppet.grahamgilbert.dev

puppet agent --test
