# Kanopi Code Test for WordPress Front-End Engineers
Welcome! Thank you so much for your interest in Kanopi Studios :herb:. This project is designed to showcase your site building approach, your front-end skills and your knowledge of a few core features of WordPress.


## The rules
1. Please spend no more than **three hours** on this project. **It's okay if you do not finish in that time.** Just make sure you provide a clear outline of what you have done, what is still to do, and any known issues.
2. Please do your work in a **fork** of this repository.
3. The timestamp of your last commit will be the cutoff time used. Any commits after the three-hour mark will not be considered as part of your submission.
4. Please use WordPress coding and documentation standards as defined in PHPCS.
6. Your solution may not rely on any third-party WordPress plugins other than those installed via Composer for this project.
7. Your work will be tested on a default WordPress installation running the theme in your fork of this repository.

## The code requirements
1. Meet WordPress coding standards ([WPCS](https://github.com/WordPress/WordPress-Coding-Standards)).
2. Meet (or exceed) [WCAG 2.1 AA accessibility guidelines](https://www.w3.org/WAI/WCAG21/quickref/?currentsidebar=%23col_customize&levels=aaa).
3. Take performance into consideration.
4. The theme must be responsive (not adaptive).
5. Your styling must take a mobile-first approach.

## Getting started
1. Download the GitHub repository.
2. Set up a local development site. We use [Docksal](https://github.com/docksal/boilerplate-wordpress) here at Kanopi. [Local](https://localwp.com/) and [Lando](https://lando.dev/) are also great. Do whatever makes you fastest!
3. Install the site's required plugins (and the theme you'll be using) with the Composer file in the root of the project.
4. Set up your theme for development. The supplied theme (`wp-vanilla`) uses `npm` and `gulp`.

### The theme uses:
* Node v10.12.0
* Gulp 3

### Running tasks
The site should Glob your JS and and SCSS together.
Right now, if you add a new SCSS partial or an new JS file you may need to stop and restart Gulp or the NPM script. We are in the process of changing this when we upgrade to Gulp 4.

1. Run `npm
1. Use `npm run watch` to watch for changes. Alternatively run `gulp watch`.
1. Use `npm run serve` to launch browserSync. Alternatively run `gulp serve`.
1. Use `npm run build` to clean and compile for PROD. Alternatively run `gulp build`.

### Notes:
* NPM does not install the gulp-cli. This theme assumes the package is installed globally.
* `package.json` and `package-lock.json` were built within a docker container.
* To use browser sync be sure to update the localUrl found here `gulp/config/browserSync.js`.

## The task

### Setup
1. Activate ACF. This should automatically load the ACF field group for events.
1. Add some terms to the Events Type taxonomy.
1. Generate some dummy events.

### Theme
1. Add the ACF fields for the Events CPT to the template file for viewing individual Events. **NOTE:** You do not need to theme this page unless you have time left over (see below).
2. Build a loop that will list only upcoming events. The loop should contain the following fields:
  * Feature image
  * Start date
  * End date
  * Title
  * Subtitle
  * Excerpt
3. [Theme the upcoming events loop to match the provided design](https://www.sketch.com/s/4f740b69-695e-4bf2-a6f7-4a8d52e76b69). The font used in this design is [Nunito Sans](https://fonts.google.com/specimen/Nunito+Sans). Use the inspector in Sketch Cloud to get the details of the layout.
3. Only the logo is an exportable asset. The event images are all [FPO](https://en.wikipedia.org/wiki/For_position_only) and can be replaced with anything you like. Note that this design is not exact and doesn't require pixel precision; however you should adhere to the grid and make it as close as possible.
3. You do not need to paginate this loop; it should just show all upcoming events in one page.

### Enhance
1. Add some JavaScript filters to to the Events archive page that lets you filter events by the following criteria:
  _We realize this can easily be done with a plugin such as FacetWP but we want to see you skills.
  * Start date (sort by closest date)
  * Taxonomy terms

## Ideas for extra fun stuff :tada:
If you have extra time and want to show off, here are some ideas!
* Because the upcoming events loop contains a meta query, cache it with a transient. Your transient should get cleared when an event is published, and when an event is updated.
* Theme out the single event page using the provided design.
* Build a past events loop that contains the same fields as above, add a transient for this loop as well.
* Create an upcoming events Gutenberg block.
* Add some snazzy animations.

## Submitting your work
When you are ready to submit your work, please send a link to your fork repository to hr@kanopi.com, katherine@kanopi.com, and shane@kanopi.com.

Good luck! We are cheering for you! Ready... set... go! :checkered_flag:
