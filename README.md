# SMB Server Files
Configurations and various files for the SMB servers
Also contains .ent file fixes where necessary


Config legend:

info-: File used to start the server, holds everything unique to this specific server, start with something like: ./xonotic-dedicated +serverconfig configs/info-servername.cfg  
auth-: Security information (rcon password, etc), should be executed from all servers you wish to share the same security details  
server-: Mode specific config, for example instagib or public CTF, should be executed from the info- file  
aliases-: Aliases and extra votes for this server, should be executed from the info- file (note: must be included after sv_vote_commands is set, if custom votes are added)  
common-: Special file, holds options shared between all servers, should be included at the top of every info- file