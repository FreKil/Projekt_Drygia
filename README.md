<h1>Drygia</h1>

<h3>Installation</h3>

<p>
	För att ladda ner och få ramverket att fungera för följande:<br />
	<ol>
		<li>Clona ramverket från följande adress https://github.com/FreKil/Projekt_Drygia.git</li>
		<li>Gör mappen och filen i site/data skrivbar genom kommandot chmod 777 mappen(dvs sökvägen till mappen)</li>
		<li>Peka sökvägen på RewriteBase i .htaccess-filen till ramverkets katalog.</li>
		<li>Gå till ramverkets startsida och logga in(inloggningslänk finns uppe till höger) med användarnamnen: root och lösenordet: root</li>
		<li>För att installera modulerna så surfar man till adressen http://ramverkets-adress/module/install</li>
	</ol>
	Ramverkets databas bör nu vara installerat och konfigurerat.
<p>

<h3>Förändra Logo/header, footer, navigation</h3>
<p>
	I filen config.php som ligger i mappen site finns möjlighet att ändra lite inställningar i ramverket. 
	Bland annat logo bilden och titeln till denna samt footer och navigationsmenyn.
</p>
<p>
	Logo/titel och footern hittas näst längst ner i config-filen. Där finns en multidimensionell array som heter config['theme'], 
	där kan diverse information om det tema som man ska använda samt hur detta ska implementeras anges och i den finns en array till som kallas 'data' där header och footer kan ändras.
	För att ändra logo-bilden anges filnamnet i variabeln 'logo_pic'. Bilden ska ligga sparad i mappen "pic" under det tema som används.
	För att ändra titeln ändras variabeln 'logo_text' och för footern ändras variabeln 'footer'.
</p>
<p>
	Navigationsmenyn finns längs ner i config-filen, i en multidimensionell array som kallas 'menu'
	Där kan olika menyer läggas till, för närvarande är det menyn 'my-navbar' som är aktiverad men kan ändras i config-filen under 'theme'
</p>
<p>
	För att lägga till fler länkar till sitt ramverk fortsätter man bara att fylla på arrayen 'my-navbar' med nya.
	'label' är själva namnet som ska visas på länken och 'url' är adressen den leder till.
	EX 'link' => array('label'=>'My Link','url'=>'link url'),
</p>
<p>
	Utöver det kan man även ändra utseendet på sin webbsida via CSS-filen som kallas style.css och ligger i mappen för varje tema.
</p>

<h3>Skapa en blogg-post</h3>
<p>
	<ol>
		<li>Logga in med root/root.</li>
		<li>Gå till bloggen.</li>
		<li>Längs ner på bloggen, klicka på länken "Create new post"</li>
		<li>Fyll i informationen i formuläret. Se till att "Type" = post. Filter bör vara plain.</li>
		<li>Klicka på "Create".</li>
	</ol>
</p>

<h3>Skapa en ny sida.</h3>
<p>
	<ol>
		<li>Logga in med root/root</li>
		<li>Gå till förstasidan eller profilen och klicka på "Create Content"</li>
		<li>Fyll i informationen. Se till att "Type" = page och filtret bör vara plain.</li>
		<li>Klicka på "Create"</li>
		<li>Ska den nya sidan synas i menyn så gå till config.php och lägg till den under "menu"</li>
	</ol>
</p>





 

