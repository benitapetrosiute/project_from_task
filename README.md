# Redmine project from task plugin

## Overview

This plugin automatically turns a task into a sub-project.

## About project
This plugin allows you to turn a task into a sub-project. When a task created in the project initiation phase is confirmed by changing the status, then the task is converted into a sub - project in the project execution phase.

## Compatibility
Redmine x.x.x compatible

## Features List
1. Task conversion into sub-project

## Plugin install
Install project_from_task plugin for Redmine

cd $REDMINE_ROOT
git clone https://github.com/AlphaNodes/project_from_task.git plugins/project_from_task
bundle install
bundle exec rake redmine:plugins:migrate RAILS_ENV=production

More information on installing Redmine plugins can be found here: http://www.redmine.org/wiki/redmine/Plugins

After the plugin is installed and the db migration completed, you will need to restart Redmine for the plugin to be available.

## Uninstall
Uninstall project_from_task

cd $REDMINE_ROOT
bundle exec rake redmine:plugins:migrate NAME=project_from_task VERSION=0 RAILS_ENV=production
rm -rf plugins/project_from_task
## Test

