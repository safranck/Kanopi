# Kanopi Code Test for WordPress Front-End Engineers
Welcome! Thank you so much for your interest in Kanopi Studios :herb:. This project is designed to showcase your site building approach, your front-end skills and your knowledge of a few core features of WordPress.


## The rules
1. Please spend no more than **three hours** on this project. It's okay if you do not finish in that time; just make sure you provide a clear outline of what you have done, what is still to do, and any known issues.
2. Please do your work in a **fork** of this repository.
3. The timestamp of your last commit will be the cutoff time used. Any commits after the three-hour mark will not be considered as part of your submission.
4. Please use WordPress coding and documentation standards as defined in PHPCS.
5. All files must be managed in a plugin.
6. Your solution may not rely on any third-party plugins other than those installed via composer for this project.
7. Your work will be tested on a default WordPress installation running the theme in your fork of this repository, and using the standard [Theme Unit Test](https://codex.wordpress.org/Theme_Unit_Test) content.

## The code requirements
1. Meet WordPress coding standards (WPCS).
2. Meet WCAG 2.1 AA accessibility standards.
3. Take performance into consideration.
4. The theme must be responsive (not adaptive).
5. Your styling must take a mobile-first approach.

## Getting started
1. Download the GitHub repository.
2. Set up a local development site. We use [Docksal](https://docksal.io/) here at Kanopi. [Local](https://localwp.com/) and [Lando](https://lando.dev/) are also great. Do whatever makes you fastest!
3. Install the site's required plugins (and the theme you'll be using) with the Composer file in the root of the project.
4. Set up your theme for development. The supplied theme (`wp-vanilla`) uses `npm` and `gulp`. Run `npm` install. Run `gulp:serve` to run `browsersync` and `watch`, or simply `gulp` to start watching for changes.


## The task

### Build
1. Register an Events custom post type.
2. Remove comments from the Events custom post type.
3. Add a Events Type custom Taxonomy.
4. Add the Events Type taxonomy to the Events custom post type.
5. Using Advanced Custom Fields, add the following fields to Events:
    1. Add a start date
    2. Add a end date
    3. Add a subtitle
    4. Add a teaser image field (yes, there's always `the_thumbnail`... but this is a test!)

### Theme
1. Add the above fields to the template file for viewing individual Events.
2. Build a loop that will list only upcoming events. The loop should contain the following fields:
  * Teaser image
  * Start date
  * End date
  * Title
  * Subtitle
  * Excerpt
3. Theme the upcoming events loop to match the provided design. You do not need to paginate this loop; it should just show all upcoming events in one page.
4. Because the upcoming events loop contains a meta query, cache it with a transient. Your transient should get cleared when an event is published, and when an event is updated.

### Enhance
1. Add some JavaScript filters to to the Events archive page that lets you filter events by the following criteria:
  * Start date
  * Taxonomy terms

## Ideas for extra fun stuff :tada:
If you have extra time and want to show off, here are some ideas!
* Build a past events loop that contains the same fields as above, add a transient for this loop as well.
* Create an upcoming events Gutenberg block.
* Add some snazzy animations.

## Submitting your work
When you are ready to submit your work, please send a link to your fork repository to hr@kanopi.com, katherine@kanopi.com, and shane@kanopi.com.

Good luck! We are cheering for you! Ready... set... go! :checkered_flag:
