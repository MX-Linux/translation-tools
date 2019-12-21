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

2018.08.07

Modified remake_desktops so that the translator does not have to put "Name=" or
"Comment=" at the start of the lines. Just translating the English name of comment
is OK.

2019.04.23

Refresh repo with latest version of all scripts.

2019.09.02

Refresh repo with latest versions.
Add desktop_driver.txt, trans_driver.txt, pushdates.odt

2019.10.04

desktop_driver.txt:    comment out mx-tweak because mx-tweak has two versions temporarily
getmxtrans:            add mr language
pushdates.odt:         updated status
remake_pkglist_des:    allow to produce differences directory and files
trans_driver.txt:      add mx-datetime, comment out mx-tweak temporarily

2019.10.24

desktop_driver.txt:     deleted # from xm-tweak
getmxtrans:		added fil_PH language
trans_driver.txt:       deleted # from mx-tweak 

2019.12.21

getmxtrans:		added bn and vi languages

