[![Formulas Scheduler (Default)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/formulas-scheduler.yml/badge.svg)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/formulas-scheduler.yml)

[![Formulas Scheduler (Container)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/formulas-scheduler-container.yml/badge.svg)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/formulas-scheduler-container.yml)

[![Formulas Scheduler (with Secrets)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/formulas-scheduler-secrets.yml/badge.svg)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/formulas-scheduler-secrets.yml)

[![Formulas Scheduler (with Dockerfile)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/formulas-scheduler-dockerfile.yml/badge.svg)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/formulas-scheduler-dockerfile.yml)

# Formulas-scheduler

Repository with a Github Action workflow example to execute specific Ritchie CLI formulas using [CRON](https://crontab.guru/#*_*_*_*_*).

It is also possible to use formulas with credentials adding [new secrets](https://docs.github.com/pt/actions/reference/encrypted-secrets) to the repository.

## A few words about Scheduled Jobs on Github Actions

When you set up a GitHub Actions workflow with a **schedule**, say for once every 10 minutes, you're essentially requesting GitHub to schedule that workflow for you. There is no guarantee that the workflow will run every 10 minutes. 

In a discussion in the GitHub Support Community ([No assurance on scheduled jobs?](https://github.community/t/no-assurance-on-scheduled-jobs/133753)), Github partner @brightran](https://github.community/u/brightran/summary) said that many times, there may be a delay when triggering the scheduled workflow:

> Generally, the delay time is about 3 to 10 minutes. Sometimes, it may
> be more, even dozens of minutes, or more than one hour.

He also said that if the delay time is too long, the scheduled workflow may be not triggered at that day. Therefore, it's not recommended to use GitHub Actions scheduled workflows for production tasks that require execution guarantee.

[Source](https://upptime.js.org/blog/2021/01/22/github-actions-schedule-not-working/)

## Docker Images with Ritchie CLI

You can find some Dockerfile examples with Ritchie installed and initialized on this [Github repository](https://github.com/GuillaumeFalourd/ritchie-docker-images) or the related Docker images on this [Docker Hub](https://hub.docker.com/repository/docker/guillaumefalourd/ritchiecli).
