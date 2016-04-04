#Contributing

In order to contribute to this project you need to have the latest version of appropriate repositories in the same directory as nodezoo-system. This will enable you to perform linking via npm.

##Set repositories up for linking

###Run for each repository
npm link nodezoo-foo (e.g. nodezoo-web, nodezoo-base)

##Linking repositories

Navigate to nodezoo-system directory

Should Contain:
*nodezoo-base
*nodezoo-info
*nodezoo-search
*nodezoo-npm
*nodezoo-github
*nodezoo-travis
*nodezoo-web

###Run
npm link ../nodezoo-web for each repository (nodezoo-info, etc.)

###Rebuild
fuge build fuge/system.yml

###Run the Project
fuge shell fuge/system.yml
