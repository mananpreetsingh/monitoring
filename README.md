# Docker Monitoring with Graphite, Graphite Beacon, collectd and Grafana

Everything is Configured as ready to go! Only **Prerequisite** is you need to have docker and docker-compose installed on your machine.
<br/> <br />

Monitoring prject contains below components: 

1. Graphite Server (To collect Metrics from collectd)

2. Grafana Server (To visualize the Metrics)

3. Graphite Beacon (To Send Alerts, Since Grafana does not has flexible Alerting system buit-in)

4. SMTP Mail server (MailDev - To Receive alert Emails)

 <br /> <br />

Follow the below steps in order to test it in your docker environment:

**Step 1:** Git clone the repository using command: `git clone https://github.com/mananpreetsingh/monitoring.git`

**Step 2:** Change your current directory to "owl" by running command `cd monitoring`

**Step 3:** Run the command `docker-compose up -d`

**Step 5:** Check everything is up and running using docker command `docker-compose ps`
 <br /> <br />

Now all you need to do is send metrics to Graphite server, for that you have run a new container with collectd service installed on it and then start the service on that contianer.

You are ready to go!
 <br /> <br />

To remove all data and containers use below commands:

	`docker-compose stop`

	`docker-compse rm -f`
