# odootools


Install by:


wget -O- https://raw.githubusercontent.com/vertelab/odootools/master/install | bash


Uninstall by: (this drops your databases and all your data related to Odoo)

wget -O- https://raw.githubusercontent.com/vertelab/odootools/master/uninstall | bash


Odoo-tools commands:

Odoo-tools command |Description
--- | --- 
 alldbs                    | Lists all databases             
 allprojects               | Lists all projects              
 cdb                       | change database                 
 cdo                       | change directory to Odoo core   
 cdp                       | change directory to project     
 odooaddons                | Updates addons_path with all project according to ODOOADDONS defined in odoo.tools
 odooadminpw               | view master password            
 odoofind <pattern>        | find patterns in odoo-core source code                     
 odoogitclone <project>    | clones and installs projects from githuh (vertel-projects)   
 odoopatch                 | Implements patches from the directory /etc/odoo/patch.d        
 odoorestart               | Restarts odoo and apache/varnish or other systems that have to be restarted (configure in odoo.tools)
 odoosync -h <host> -p <project> | Syncs a project to a server without git meta data           
 odootail                  | Views odoo-log live, you can use the one-liner *odoorestart ; odootail* to restart and monitor odoo
odooupd -h, --host=	host -P, --port=	port  -d, --database=	database -m, --module=	comma separated  module list   -p, --password= admin password   -l, --list	list all modules   -i, --install	install or upgrade modules  -u, --uninstall	uninstall modules | Modifies Odoo-instanses
odooupdm <database> <modulelist>      | Installs/updates modules in single user mode                
 odoovilog                 | Opens Odoo log file in vi       
 
