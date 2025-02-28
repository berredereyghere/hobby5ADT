# Hobby5ADT

---

### Info over mijn hobby:
Mijn hobby is alles met computers doen. Ik vindt hardware heel leuk maar ook alles wat je kan configuren. In Linux, macOS of Windows. De laatste tijd ben ik heel veel bezig met een proxmox server intestellen. Ik zit nu al aan 14 lxc's die aan het draaien zijn. En ik ben nog niet eens begonnen an virtual machines. Ook vindt ik netwerken heel leuk. Ik heb al geprobeerd om opnwrt te installen op proxmox. Maar dat heeft het netwerk een beetje kapot gemaakt dus heb ik het snel verwijdert. Kortom ik vindt alles met computers zeer leuk en intersant.

---

### Mijn favoriete activiteiten van mijn hobby:

- Ik vindt het heel leuk als je net een nieuwe container/lxc/vm hebt opgezet en je mag hem configureren via een web gui. 

- Ik vindt het ook zeer leuk om veel tijd te steken in dashboards.

- Wat ook leuk is als je een dashboard hebt kunnen installeren en je moet nog heel veel zelf doen. Zoals bij home assistant.

---

### Hoe installer ik homeassistant op een proxmox server?

1. Eerst begin je met een lxc aan te maken in proxmox. *(Je kan ook gebruik maken van een vm. Maar die gebruiken meer resources en duren langer om op te zetten.)* Je kan kiezen van welke distributie. Ik persoonelijk vindt Ubuntu/Debian de beste omdat het heel stabiel is en omdat ik die het meest gebruikt. CentOS heb ik nog nooit geprobeerd.  

2. Nu dat je je lxc hebt gemaakt. Log je in op proxmox in je lxc. Of als je het ip address al weet ssh gebruiken.

3. Nu dat je de lxc gemaakt hebt en verbonden bent gaan we docker installeren om homeassistant te installeren. Docker kan je gemakkelijk installeren met hun script dat op hun website staat.

4. Nu hebben we docker geinstallerd. Ik gebruik graag een extra gui. Dus is dit een extra stap die onodig is. Daarom zullen we portainer installeren. Dit die je met het command "docker pull portainer" als je dit command het uitgevoerd zal je de portainer container gemaakt worden. Dan zal normaal zien dat het aan het runnen is met "docker -ps". Als hij aan het runnen is, kan je naar je browser gaan en dan het ip intypen en dan ":9443" dus het totaal plaatje ziet er al volgd uit: [je ip]:9443.

5. Nu dat we portainer hebben geinstallerd kunnen we beginnen met homeassistant te installeren. Ga naar portainer log in, en druk op "stacks". Dan kan je de stack invoegen die op de homeassistant website staat. Als je de stack hebt toegevoegd. Kan je dan op deploy drukken en dan zal normaal de homeassitant container gemaakt worden. 
6. Nu hebben we homeassistant geinstallerd. Je kan er naar toegaan via [je ip]:8123 

