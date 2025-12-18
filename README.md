# Catch the Balloon (Pràctica Robòtica Assistencial)

Joc didàctic desenvolupat a Unity amb suport d'interacció robòtica orientat a nens amb dificultats cognitives i atencionals.
El projecte utilitza diferents reptes educatius per treballar l'atenció, la memòria, el raonament lògic i la motivació, amb el robot actuant com a guia i reforç positiu.

Adrià Romo, Alba Rey i Berta Fornols

---

## Execució del Joc
Hi ha la possibilitat d'executar el codi des de la plataforma Unity. 

Primer de tot, s'ha d'obrir el simulador del robot.

A dins del Unity, s'ha de clicar el botó d'inici on et portarà a les configuracions bàsiques, allà s'ha d'omplir el nom i la IP que hagi mostrat el robot. En el cas de la dificultat, independentment del que se seleccioni el joc actuarà igual.

Un cop s'ha establert connexió, s'ha d'obrir el teacher controller, i apuntar la IP que ens hagi mostrat el joc.

En aquest moment tindrem la comunicació mitjançant sockets entre dispositius.

Ara el robot inicialment parlarà amb l'usuari abans de començar el joc, per això polsarà el botó de la mà per iniciar la interacció, cada vegada que l'infant respongui, es pot interactuar amb el teacher controller, amb els botons superiors de tics i creus.

Una vegada el robot, pregunti si està a punt per jugar, ja es podrà tornar a polsar el botó de la mà per començar el joc.

El primer repte que es mostrarà, consisteix a polsar els globus per pantalla que sumin el valor que el robot hagi escollit, sempre l'infant ha d'esperar que el robot respongui abans de polsar un altre globus.

Un cop completi el repte numèric correctament, passarà el següent nivell. En aquest cas s'ha intentat implementar un laberint, però per motius que no hem sabut trobar, no hem aconseguit que es mostrés la imatge del laberint. Tot i això, hem deixat el repte per mencionar que s'ha intentat la seva execució. En aquest cas sí que és el teacher controller, el que mitjançant el botó verd haurà d'indicar quan l'infant hagi aconseguit sortir del laberint, o el vermell en cas incorrecte.

Els següents dos reptes funcionen amb interacció altre cop com els números, un en el qual es mostraran globus de diferents colors i l'infant haurà de seleccionar el color que el robot hagi mencionat. I un últim repte en el qual es busca la capacitat de memòria, on s'ha de seleccionar les parelles amagades darrere els globus.

En aquests dos reptes, no és necessari la interacció del robot, per poder indicar que s'ha completat, ja que el joc ja té la lògica necessària. 

Un cop hagi completat l'últim repte correctament, el robot demanarà si vol ballar, el qual el teacher controller haurà d'indicar en cas de voler fer-se.

Un cop s'acabi el ball, el joc finalitzarà l'execució i podrem desconnectar el robot i el teacher controller.

L'altra manera d'executar seria directament amb l'executable des d'un dispositiu Windows. El qual el procediment seria exactament el mateix, però en aquest cas el joc es duria a terme sense haver de fer servir el Unity.

