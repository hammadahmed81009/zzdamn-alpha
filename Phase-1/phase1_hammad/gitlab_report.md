# Exploring Gitlab CI/CD

## Introduction

This report summarizes my hands-on experience with GitLab CI/CD for a sample Node.js project. I configured CI/CD pipelines to run install tasks on repository events.

## Overview

Key components used:

- GitLab CI/CD for defining pipelines in YAML
- GitLab runner to execute pipeline jobs
- Git repository with Node.js code

## Hands-on Experience

I followed these steps to set up the project:

- Cloned the ts-micro-apprepo from GitHub using SSH.
- Changed directory into the repo.
- Checked out tag p1.3 to access a specific commit.
- Created a .gitlab-ci.yml  file with a yarn\_install job under the installstage.
- Added rules to trigger the job on commits to main and merge requests.
- Configured a GitLab runner to run the pipeline.
- Pushed a commit to main which triggered the yarn\_install job.

## Key Features

- git clone and git checkout commands can be used in CI/CD jobs.
- Rules provide control over when jobs run based on Git events.
- Stages organize related jobs into workflows.
- Runners enable executing non-Docker jobs.

## Final Thoughts

I found GitLab CI/CD provides an easy way to automate tasks around Git events. The pipeline was simple to implement for a Node.js codebase.