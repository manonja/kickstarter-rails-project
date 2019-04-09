# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

name    Path           HTTP Verb       Purpose                   AR CRUD method       SQL

index   /projects       GET      Display all projects      Project.all          SELECT * FROM projects

show    /projects/:id   GET      Show info one project     Project.find(params[:id]) SELECT * FROM     projects where id=1

new     /projects/new   GET      Show new project form

create  /projects       POST     Create new project, redirect  Project.create(projects_params) INSERT INTO projects(name) VALUES(params)

edit    /projects/:id/edit  GET  Show edit form

update  /projects/:id   PATCH    Update one project, redirect  Project.update(projects_params)  UPDATE projects SET(name = 'bla') WHERE id=1

destroy  /projects/:id/delete  DELETE   Delete one project, redirect Project.destroy(id)        DELETE FROM projects WHERE id=1         
