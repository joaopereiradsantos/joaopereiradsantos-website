---
title: Tennis Betting Bot
summary: Automated Web Scraper and Value Betting Algorithm
tags:
- Betting Bot
- Web Scraping
date: "2021-10-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by Ryan Searle on Unsplash
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: Private Repo
  url: https://github.com/joaopereiradsantos/tennis-betting-bot
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

# Tennis Betting Bot

TBB is an automated web scraping bot that scrapes both a Crystal Ball match probability forecast and ‘oddsportal.com’ next tennis matches for bookmaker odds.

The bot preprocesses both outputs and if the bet is considered valuable, an email is sent with informations regarding the players, crystal_ball_odd and bookmaker_odd.

Next steps consist in further financial analysis from October 2021 until the end of the current season and, if successful, an automated betting.

## AWS Production Environment
### EC2 Deployment
TBB is currently in production using AWS Account with EC2 Virtual Server in the Cloud. Fully managed by the repository owner, using EC2 tree tier t2.micro, 1GB RAM, 30GB EBS with Windows 10 and Task Scheduler running .bat file at a scheduled datetime (currently 1h interval).

### T2 Instance & CPU Credit Management
The t2 operates as a Burstable Performance Instances providing a baseline CPU performance under normal workload. But when the workload increases Burstable Performance Instances have the ability to burst, i.e. increase the CPU performance. CPU Credit regulates the amount CPU burst of an instance. You can spend this CPU Credit to increase the CPU performance during the Burst period. Suppose you are operating the instance at 100% of CPU performance for 5 minutes, you will spend 5(i.e. 5\*1.0) CPU Credit. Similarly if you run an instance at 50% CPU performance for 5 minutes you will spend 2.5(i.e. 5\*0.5) CPU Credits. CPU Credit Balance is simply the amount of CPU Credit available in your account at any moment. 

Since the t2.micro elavates the CPU Utilization up to 50-75% while running the script, a CPU Credit management system was developed in order to avoid null CPU Credit available at the scheduled time. The solution orchestrates two lambda functions: ec2-stop-instance and ec2-start-instance and the same two CloudWatch Rules. The above functions are set to trigger according to the following cron expressions: 30 */12 * * ? * (stop) and 35 */12 * * ? * (start) (5 minutes after stopping the instance).

## Contributing
TBB is currently a closed source invitation only project.


## License
[MIT](https://choosealicense.com/licenses/apache-2.0/)