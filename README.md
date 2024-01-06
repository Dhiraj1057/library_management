## Library Management

Purpose of this app was learning. This is basic tutorial on frappe framework. This is made based on frappe framework tutorial library management system.
There is some help guide below. Have a look.

Installation Guide
	url: https://github.com/D-codE-Hub/Frappe-ERPNext-Version-15--in-Ubuntu-22.04-LTS/blob/main/README.md
	url: https://github.com/nvm-sh/nvm/blob/master/install.sh

	Command: bench new-site library.test
	Description: This will create new site.
	
	Command: bench drop-site library.test
	Description: This will delete new site.
	
	Command: bench --site library.test add-to-hosts
	Description: This will add library.test address to host file.

	Command: bench use library.test
	Description: This will set default site of that bench.


Usage Guide
	Cheatsheet: https://frappeframework.com/docs/user/en/bench/resources/bench-commands-cheatsheet

	Command: bench new-app library_management
	Description: This is command for creating new app.

	Command: bench --site library.test install-app library_management
	Description: This will install application inside given site.

	Command: bench --site library.test list-apps
	Description: For checking all app inside given site.

	Command: bench --site library.test console
	Description: This is python console for given site.

	Command: bench --site library.test mariadb
	Description: This is mariadb console for given site.
		Description: ${} is used for template literal in below code

		Command: desc tab${Artticle};
		Description: It will tell detail description of that form

		Command: select * from tab${Article};
		Description: To get all of data in that form

	Command: bench --site library.test backup
	Description: Database Backup

	Command: bench --help
	Description: You can see a list of all site commands by running the following command:

	Command: bench set-config -g developer_mode true
	Description: Before we can create DocTypes, we need to enable developer mode on our bench. This will enable boilerplate creation when we create doctypes and we can track them into version control with our app.

	Command: bench --site &lt;your_site&gt; set-config server_script_enabled true
	Description: To enable server side scripts. Then, restart bench.

Thing to Learn
	--> Model: DocType is analogous to a Model in other frameworks. Apart from defining properties, it also defines the behavior of the Model.

#### License

mit


