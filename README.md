<h1>Drygia</h1>

<h3>Installation</h3>

<p>
	För att ladda ner och få ramverket att fungera för följande:<br />
	1: Clona ramverket från följande adress https://github.com/FreKil/Projekt_Drygia.git<br />
	2: Gör mappen och filen i site/data skrivbar genom kommandot chmod 777 mappen(dvs sökvägen till mappen)<br />
	3: Peka sökvägen på RewriteBase i .htaccess-filen till ramverkets katalog.<br />
	4: Gå till ramverkets startsida och logga in(inloggningslänk finns uppe till höger) med användarnamnen: root och lösenordet: root<br />
	5: För att installera modulerna så surfar man till adressen http://ramverkets-adress/module/install<br />

Ramverkets databas bör nu vara installerat och konfigurerat.
<p>

Förändra Logo/header, footer, navigation
*****************************************

I filen config.php som ligger i mappen site finns möjlighet att ändra lite inställningar i ramverket. 
Bland annat logo bilden och titeln till denna samt footer och navigationsmenyn.

Logo/titel och footern hittas näst längst ner i config-filen. Där finns en multidimensionell array som heter config['theme'], 
där kan diverse information om det tema som man ska använda samt hur detta ska implementeras anges och i den finns en array till som kallas 'data' där header och footer kan ändras.
För att ändra logo-bilden anges filnamnet i variabeln 'logo_pic'. Bilden ska ligga sparad i mappen "pic" under det tema som används.
För att ändra titeln ändras variabeln 'logo_text' och för footern ändras variabeln 'footer'.

Navigationsmenyn finns längs ner i config-filen, i en multidimensionell array som kallas 'menu'
Där kan olika menyer läggas till, för närvarande är det menyn 'my-navbar' som är aktiverad men kan ändras i config-filen under 'theme'

För att lägga till fler länkar till sitt ramverk fortsätter man bara att fylla på arrayen 'my-navbar' med nya.
'label' är själva namnet som ska visas på länken och 'url' är adressen den leder till.
EX 'link' => array('label'=>'My Link','url'=>'link url'),

Utöver det kan man även ändra utseendet på sin webbsida via CSS-filen som kallas style.css och ligger i mappen för varje tema.


Skapa en blogg-post
*******************
1: Logga in med root/root.
2: Gå till bloggen.
3: Längs ner på bloggen, klicka på länken "Create new post"
4: Fyll i informationen i formuläret. Se till att "Type" = post. Filter bör vara plain.
5: Klicka på "Create".

Skapa en ny sida.
******************
1: Logga in med root/root
2: Gå till förstasidan eller profilen och klicka på "Create Content"
3: Fyll i informationen. Se till att "Type" = page och filtret bör vara plain.
4: Klicka på "Create"
5: Ska den nya sidan synas i menyn så gå till config.php och lägg till den under "menu"





 

