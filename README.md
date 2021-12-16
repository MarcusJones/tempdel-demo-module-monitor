# tempdel-demo-module-monitor

This is a list of modules that have been updated to latest spec, tested individually and tested with data services on weeve Agent:

hash-to-int :white_check_mark:

http-egress :white_check_mark:

dev-random :white_check_mark:

mqtt-ingress :white_check_mark:

slack-alert :white_check_mark:

weevagator :white_check_mark:

cleaner/sweeper :white_check_mark:

filter :white_check_mark:

vonage-alert :white_check_mark:

dynamodb-egress :white_check_mark:

batcher :white_check_mark:

http-ingress (tested individually  :white_check_mark:, but NOT tested with weeve Agent yet as waiting for ports bindings to be fixed :x: )

This is a list of modules that I did not update:

file-watcher :x: (@marcus.jones maybe some pair programming? I don’t really understand this module)

ocr :x: (no access to the camera setup for testing, waiting for @Sanyam Arya to return)

dog-vs-cat / Tensorflow :x: (no access to the camera setup for testing, waiting for @Sanyam Arya to return)

camera-capture :x: (no access to the camera setup for testing, waiting for @Sanyam Arya to return)

Hello-Weeve :x: (part of the published documentation, so no need to update as there is a slightly different purpose of that module)

I need somebody to accept all of the following merge requests:

13 Modules MR: https://gitlab.com/groups/weeve/modules/-/merge_requests

Modules’ YAMLs in Manager Utilities: https://gitlab.com/weeve/admin-utilities/manager-utilities/-/merge_requests/35

Moreover, I need @marcus.jones or @Sanyam Arya to push the latest versions of the modules (after MRs are accepted) to DockerHub, because I don’t have credentials 
to do it.

If @channel needs to use modules for any testing before they would be published to DockerHub, then pull modules from GitLab and run make create_image to create a 
local copy of the image, so that weeve Agent uses a working local copy rather than pulling old modules from DockerHub. (edited) 



