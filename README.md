Winnie
====================================
Winnie är ett MVC inspirerat ramverk för webbutveckling. 
För att se ramverket gå till: <code>http://www.student.bth.se/~mili13/phpmvc/kmom08/lydia/</code>
För att logga in:

______________________
Username: doe

Password: doe
____________

eller
__________
Username: root

Password: root
______________________
Du kan även skapa ditt egna konto och logga in.

För att skapa ett eget ramverk som Winnie är det bara att följa följande steg:

Installation
-------------

1. Clona Winnie från github: <code>https://github.com/mili13/kmom08.git</code>
2. Gör site/data skrivbar: <code>cd lydia; chmod 777 site/data</code>
(Både mappen och filen i mappen måste vara chmod 777)
3. Öpnna .htaccess filen, och ändra länkningen till:
 <code>RewriteBase /~mili13/phpmvc/kmom08/lydia/</code>
4. Peka din webbläsare till din Winnie och följ instruktionerna.
<code>module/install</code>

Ändra logga, titel, footer och navigations menyn
--------------------
Öppna filen: 
<code>lydia/site/config.php</code>

Skrolla ner till "Settings for the theme. The theme may have a parent theme."
<code>$sk->config['theme'] = array(</code>

Här kan du ändra logga, titel, footer och menyn

Om du vill ändra utseendet på ramverket kan du gå till:
<code>lydia/site/themes/mytheme/style.css</code>


Skapa en ny blogg-post
--------------------

För att skapa en ny blogg-post gör följande:


1. Öppna ramverket i din webbläsare
2. Clicka på "blog"
3. Clicka på "edit" 
4. Clicka på "create new"
5. Skapa en ny blog.Säkerställ att "Type" är "post", and Filter är "plain"
6. spara


Skapa en ny sida
--------------------

1. Öppna ramverket i din webbläsare
2. Clicka på "About me"
3. Clicka på edit
4. Clicka på "Create new"
5. Clicka på "spara" när du är klar

Om du vill att en ny sida ska synas i menyn gör följande:

1. Öppna filen <code>lydia/site/config.php</code>
2. scrolla ner till "Define menus."
3. lägg till en rad i slutet av <code>'my-navbar' => array(</code>

Exempel -> <code>'page' => array('label'=>'page', 'url'=>'page/view/9'),</code>


