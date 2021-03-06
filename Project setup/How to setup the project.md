When creating a project on bitbucket or github, it is paramount to specify few crucial details for project setup. This will help with quick onboarding of new developers on the project.

In the project root folder there should be a `README.md` file. At the beginning of this file you should give few details about the project and details about the development setup.

A sample readme should look like this:

```md
# Development and deployment

Project _project_ is the project about stuff and some other stuff.

## Development environment

 * **Development URL:** http://dev.projectname.org
 * **Development database:** database_name
 * **Database prefix:** db_

## Staging server
 * Staging server pulls code from `development` branch

## Preproduction server

  * staging branch
  * preproduction ready features, test on actual content
  * **DON'T OVERRIDE THE DATABASE**

## Production server
  * master branch
  * only production ready features
  * **DON'T OVERRIDE THE DATABASE**

## Additional details

For theme quick start check [wp-boilerplate](https://github.com/infinum/wp-boilerplate) readme.

Mention some additional details here. For instance if you have any special deployment techniques from development to staging, additional constants and settings for `wp-config.php` or similar.
```

Never write data which is meant to be secure in your readme file, or commit them directly to the repository.
