---
title: Repo Naming Guidelines
layout: /page.*

---

# Repo Guidelines

Below are the guidelines for naming a repository in xmidt-org.  We have four 
primary types of repositories: 

- **deployment** - Contain the files needed to deploy a project as well as the
                   integration tests.
- **servers** - Contain the docs and code that builds into a specific service
                that can be run.  Each server is part of a project, so there may
                be different guidelines for different projects.
- **libraries** - General code that don't build into a service that can be run;
                  instead, they are imported by the server code.  Libraries can
                  be used by multiple projects.
- **docs** - A singleton repo, which harvests documents from other repos and
             provides overall documentation that doesn't fit well somewhere
             closer to the code.

## General

- No profanity or otherwise inappropriate language.
- Words used should not be copyrighted, trademarked, or otherwise associated 
  with prominent code that already exists.
  - An example of not following this guideline would be called a repo `viper`,
    despite the prominent golang `viper` repo that already exists.
- The name should be meaningful and relate to what the code does.

## Deployment

- Deployment repos for a project should be the name of the project followed by 
  "deploy". Ex: `codex-deploy`
- Deployment repos for a specific server should be the name of the server 
  followed by "deploy".  Ex: `svalinn-deploy`

## Servers

- XMiDT servers should have names that are meaningful within ancient
  Greek mythology.
- Codex servers should have names that are meaningful within ancient Norse 
  mythology.
- Webpa servers should have names that contain some form of '181' in the name.
  Leetspeak names are ok.

## Docs

- Documentation should be kept as close to the code as possible, in the same 
  repo.

## Other

- A repo that belongs to a project should have that project's name as a topic.
- The short description of a repo should include what type of repo it is.
- A repo that holds Golang code may have dashes in it, but the go packages 
  should not and any outputs should not (like binary names).
