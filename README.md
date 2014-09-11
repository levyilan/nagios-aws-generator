Simple PHP library which will help you generate hosts and services nagios files for nagios3


 In order to use this, you need to export two variables:

 export AWS_KEY=YOUR_AWS_ACCESS_KEY

 export AWS_SECRET=YOUR_AWS_ACCESS_KEY_SECRET



 Run in the console:

 php generate.php



 The generator will find all of your instances which have tag "nagios" no matter what the value is.

 The proper value could be:
 check_load

 or if you wish to have more than 1 service checked on that instance:

 check_load|check_root_partition


 You need template file called service.check_load.template in the templates folder.

 You can create template files based on your setup.
