# pcfwebdemo



## How to deploy to cloudfoundry

Prerequisite : you must have a pivotal account

- Go under the folder where the war has been exported.

- Connect to cloud foundry using `cf login -a https://api.run.pivotal.io`

- Select the space you want to deploy to

- `cf push -p pcfwebdemo.war`

Remark : you may have to add `-m 64M` on test environment if you don't have enough memory and `-k 256M` for disk space


Test the application [pcfwebdemo](http://pcfwebdemo.cfapps.io)