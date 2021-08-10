# Services that use the Slack webhook
1. The Elastalert configs on prod and dev log aggregators:
	- /home/ubuntu/heavens-docker/ara/elastalert/rules/errorAlertToSlack*
	
2. The disk usage script on DLU prod
	- /home/kpmp-appuser/diskUsageCheck.sh
	
3. Uptime Robot:
	- https://uptimerobot.com/dashboard?ref=website-header#mySettings --> Alert contacts
	
4. The Docker container checker .env file
	- Wherever the docker_container_check.py script is, e.g. /home/ubuntu or /home/kpmp-appuser
