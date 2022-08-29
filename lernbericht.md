# Lern-Bericht
Elias Gössi

## Einleitung

Wir bearbeite das Modul 133, indem wir Web-Applikationen mit Session Handling realisieren.

## Was habe ich gelernt?

Ich habe gelernt, wie ich mit JSF ein Bild, gleichzeitig als Element und als Link verwenden kann.

## Beschreibung

Man hat mehrere Möglichkeiten, um von einer auf die nächste Webseite zu wechseln, zum Beispiel mit einem Link, einem Button oder sogar einem Bild.
Wir haben zwei Bilder auf der Startseite und beide Bilder sollen zu einer anderen Webseite führen. Damit wir nicht einen zu grossen Aufwand haben, sollen beide Bilder zur gleichen Seite führen und nur der Inhalt soll je nach ausgewähltem Bild angepasst werden.
Also muss gemerkt werden, welches Bild ausgewählt wurde, das legen wir mit `target="#{helloManagedBean.favourite}" value=""` fest. 
Egal welches Bild wir jetzt auswählen, kommen wir auf die "zweite" Seite und nur der Inhalt wird je nach Bild angepasst.


```java
<h:commandLink value="" action="seite2.xhtml">
    <f:setPropertyActionListener target="#{helloManagedBean.favourite}" value="links" />
    <h:graphicImage library="img" name="IMG_1.jpeg" width="200"/>
</h:commandLink>

<h:commandLink value="" action="seite2.xhtml">
    <f:setPropertyActionListener target="#{helloManagedBean.favourite}" value="rechts" />
    <h:graphicImage library="img" name="IMG_2.jpeg" width="200"/>
</h:commandLink>
```

![image](https://user-images.githubusercontent.com/54137474/187169559-90fd8e9f-0013-468a-ade9-cc3bf28d6899.png)


## Verifikation
Der Text beschreibt weshalb und wie man Bilder als Link verwenden kann. 
Der Code zeigt es wie man es anwenden kann und der Screenshot zeigt es noch graphisch.

# Reflektion zum Arbeitsprozess

Ich konnte die Zeit gut einteilen und konnte die Aufträge in der Schule erledigen.
Ich hatte keine Probleme, die Facelets zu erstellen und mich zwischen den Facelet-Seiten zu navigieren.


Ich hatte bis jetzt nur leichte Schwierigkeiten mit dem NetBeans, das es den Glassfish Server nicht immmer erkennt, ansonsten verlief alles gut. 

**VBV**: 
Ich würde an meinem Vorgehen noch nichts ändern, da ich momentan zufrieden bin.
