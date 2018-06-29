# translation-tools
Scripts to assist the MX translation coordinator

2018.06.29

Initialized with these scripts:

	remake-actions
	remake-desktops
	remake-services

These 3 scripts deal with pasting together translated Transifex language files
in text format. (In QT, shell, and Python apps, the Transifex files exist as
distinct files for the apps to use. But the text files need to be consolidated.)

remake-actions  creates a file that can be used to update uca.xml for Thunar
                custom actions.

remake-desktops creates a file that can be used to update the individual app's
                .desktop file.

remake services creates a file that can be used to update the services.list file
                used by the Gazelle installer.

2018.06.29

Added this script:

	getmxtrans

It displays a list of MX resources on Transifex, and downloads a standard set of
language files for the selected resource.

2018.06.29

Added this script:

	makemofiles

It takes the downloaded Transifex shell or Python translated files, puts them into
a po/ directory, and creates the "object" files, putting them in separate
language directories under a mo/ directory.
