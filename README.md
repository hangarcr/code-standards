
## License:

All content licensed under Creative Commons Attribution 3.0 Unported License

## Branch Updates




## Summary:


## Structure of Page Content

The index.html file is generated via grunt, including each of the .html files contained within the /sections/[lang] directory. We have separated the different sections that make up the page into individual files so that it is easier to edit, basically making the content of the page more modular. This is also part of what we consider a best practice when dealing with large projects, as if it were an application involving lots of code, that several people work on. index.html is then served via jekyll using the layout located in _layouts/main.html.

Each of these files include content wrapped within sections. This should be self-explanatory I think. In each section, we make use of all h1-h6 heading tags multiple times since HTML5 lets you use as many as you like. Of course, we try to always use them and all other HTML5 tags appropriately, and making use of semantic tags where they are best suited.

To edit the main layout, edit the file in _layouts/main.html, to edit the content edit the relevant section in the sections folder. Do not edit index.html.

## Getting Started with the Build process

Prior to running these commands, make sure you have ruby 1.9.3 installed, ideally using RVM.

Run 'npm install' from the command line of the project directory to install all the node dependencies. You may need to occasionally re-run this command as new dependencies are added.

Run 'bundle install' from the command line of the project directory to install ruby's dependencies. This will allow you to build the jekyll site similiar to what we are hosting on github pages, and to run the server locally. If you get a 'command not found' error, run 'gem install bundler' then try again.

Run 'grunt' from the command line of the project directory to run the build process.

To run the jekyll server locally run 'jekyll serve --watch' from the command line. You can then view the site at localhost:4000. Don't forget the '--watch' option as this enables auto-regeneration of the code.

We currently use the default jekyll configuration, so there is no configuration file.


