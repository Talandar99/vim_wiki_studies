### Access Control Lists
##### Zarówno filmik jak i strona zawierają to samo czyli kompletny opis tego jak na linuxie działają uprawnienia, uzupełniająco dorzuciłem jeszcze arch wiki jakby ktoś uznał że tłumaczenia z 2 pierwszych linków są niewyczerpujące
- Strona:https://linuxhandbook.com/linux-file-permissions/
- YT:https://www.youtube.com/watch?v=k1yzI7c6Fzk
- ArchWiki:https://wiki.archlinux.org/title/Access_Control_Lists

##### koemndy
- getfacl - get file access control lists
- setfacl - set file access control lists
- chmod - change mode (rwx access)
- chown - change owner

### Chmod 0750 i Chmod daje te same uprawnienia a dokładnie:
##### Chmod 0750 
- chmod a+rwx,g-w,o-rwx,ug-s,-t 
- sets permissions so that: 
	- (U)ser / owner can read, can write and can execute. 
	- (G)roup can read, can't write and can execute. 
	- (O)thers can't read, can't write and can't execute.

##### Chmod 750
- chmod a+rwx,g-w,o-rwx  sets permissions so that:
	- (U)ser / owner can read, can write and can execute. 
	- (G)roup can read, can't write and can execute. 
	- (O)thers can't read, can't write and can't execute.
