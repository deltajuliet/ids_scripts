# ids_scripts


_init_scripts_
Place these files in /etc/init.d to maintain suricata and daemonlogger:

daemonlogger
	Supports the following methods:
	-start
	-stop
	-restart
	-purge_pcaps
	
	If daemonlogger_rename variables are not set then files won't be renamed and will remain with epoch timestamp

suricata

	Supports the following methods:
	-start
	-stop
	-update_rules
	-restart
	-purge_rules



_utils_
These utilities can be used with the above scripts to streamline/enhance management of ids tools

daemonlogger_inotify_renamer.sh
	Requires inotify-tools to be installed to watch for newly created files