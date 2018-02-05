
#Configuration Management

<h2>Screencast</h2>

[Configuration Management](https://youtu.be/hSqp-541UlY)

<h3> Roles used</h3>
<h4> Role -> coffeeRole : To start the Coffeemaker server</h4>
<h4> Role -> seleniumRole : To implement Selenium Testing</h4>

<h3>SetUp</h3>
<h4>We need 3 vagrant machines<h4>
<h5>1. Ansible Server </h5>
<h6>Consists of both roles and play.yml file</h6>
<h5>2. CoffeeMaker </h5>
<h6>Increase the virtual memory to 2048 because server needs memory. Copy the private key .vagrant folder into Ansible-Server/keys and change the permission to 600 using chmod 600 CoffeeMaker_private_key<h6>
<h5>3. Selenium Server </h5>

<h3> Once setup is completed, execute following command:</h3>
<h4> ansible-playbook -i inventory play.yml -vvv</h4>


