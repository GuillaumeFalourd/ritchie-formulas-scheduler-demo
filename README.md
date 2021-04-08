[![1 - Formulas Scheduler (Default)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/1-formulas-scheduler.yml/badge.svg)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/1-formulas-scheduler.yml)

[![2 - Formulas Scheduler (Secrets)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/2-formulas-scheduler-secrets.yml/badge.svg)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/2-formulas-scheduler-secrets.yml)

[![3 - Formulas Scheduler (Dockerfile)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/3-formulas-scheduler-dockerfile.yml/badge.svg)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/3-formulas-scheduler-dockerfile.yml)

[![4 - Formulas Scheduler (Container)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/4-formulas-scheduler-container.yml/badge.svg)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/4-formulas-scheduler-container.yml)

[![5 - Formulas Scheduler (Action)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/5-formulas-scheduler-action.yml/badge.svg)](https://github.com/GuillaumeFalourd/formulas-scheduler/actions/workflows/5-formulas-scheduler-action.yml)

[![6 - Formulas Scheduler (Remote Dispatch)](https://github.com/GuillaumeFalourd/ritchie-formulas-scheduler-demo/actions/workflows/6-formulas-scheduler-remote-dispatch.yml/badge.svg)](https://github.com/GuillaumeFalourd/6-ritchie-formulas-scheduler-demo/actions/workflows/formulas-scheduler-remote-dispatch.yml)

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

## Ritchie Actions

You can find [Ritchie CLI actions on Github Marketplace](https://github.com/marketplace?type=actions&query=ritchie)!

- [Ritchie Action Shell](https://github.com/GuillaumeFalourd/ritchie-action-shell)
- [Ritchie Action Python](https://github.com/GuillaumeFalourd/ritchie-action-python)
- [Ritchie Action Node](https://github.com/GuillaumeFalourd/ritchie-action-node)
- [Ritchie Action Java 8](https://github.com/GuillaumeFalourd/ritchie-action-java-8)
- [Ritchie Action Go 15](https://github.com/GuillaumeFalourd/ritchie-action-go-15)
