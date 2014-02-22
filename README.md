puppetmaster clients for orawls,oradb modules
=============================================

use puppet client 3.4.3

vagrant up oradb

vagrant up adminwls or nodewls1 or nodewls2

vagrant ssh adminwls or nodewls1 or nodewls2 or oradb


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
