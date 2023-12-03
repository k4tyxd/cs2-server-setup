# cs2-server-setup

Automate the setup of Counter-Strike 2 Dedicated Server using Ansible, install plugins and configure the server settings.

## Getting started

```shell
ansible-playbook -i hosts.yaml cs2server.yaml -v
```

To use Metamod, you need to edit the gameinfo.gi file.  
Manually edit the gameinfo.gi file due to its inconvenient handling.

```diff
@@ -20,6 +20,7 @@
 		{
 			Game_LowViolence	csgo_lv // Perfect World content override

+			Game    csgo/addons/metamod
 			Game	csgo
 			Game	csgo_imported
 			Game	csgo_core
```
