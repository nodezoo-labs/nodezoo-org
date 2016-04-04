#Contributing

If you are interested in contributing to this project then you will need to have access to all the applicable repositories in order to make appropriate changes. When you run npm install on nodezoo-system it will install all of the required node modules as normal. However in order to make changes to some of these you will need to have the latest version of these repositories on your development system.

At time of writing:
nodezoo-base
nodezoo-info
nodezoo-search
nodezoo-npm
nodezoo-github
nodezoo-travis
nodezoo-web

Having the latest version of these repositories in the same directory as nodezoo-system will enable you to perform linking via npm. We will show you how to do this now.

##Set repositories up for linking

In your root directory that contains all of the repositories you should run the following command for each of the repositories

npm link nodezoo-foo #where foo is the name of the module e.g. nodezoo-web, nodezoo-base etc.

Once this is done you then need to link them.

##Linking repositories

Navigate to your nodezoo-system directory and run the following command for each of the repositories (the assumption here is that all repositories are in the same directory) - if not you will need to navigate into each directory in nodezoo-system/node_modules do it from within

npm link ../nodezoo-web

Once this is completed for each of the repositories you must rebuild

fuge build fuge/system.yml

Now you are ready to run the project.
