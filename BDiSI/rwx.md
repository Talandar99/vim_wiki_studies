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

### Chmod 0750 i Chmod 750 daje te same uprawnienia a dokładnie:
- chmod a+rwx,g-w,o-rwx,ug-s,-t 
- sets permissions so that: 
	- (U)ser / owner can read, can write and can execute. 
	- (G)roup can read, can't write and can execute. 
	- (O)thers can't read, can't write and can't execute.

##### dlaczego Chmod 0750 ?
1. Konwencja. Przez bardzo długi czas pisało się 4 symbole ze względu na to jak zapisywana w pamięci jest informacja
2. ktoś już zadał na stacku pytanie o to dlaczego jest nam potrzebny pierwszy digit więc przeklejam: 
  - https://serverfault.com/questions/344544/what-is-the-first-digit-for-in-4-digit-octal-unix-file-permission-notation
3. Ten trzeci bit to tak zwany sticky bit. Więcej o nim tutaj:
  - https://www.thegeekstuff.com/2013/02/sticky-bit/

