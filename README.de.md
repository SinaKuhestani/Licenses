# How to Choose a License for Your Own Work
[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/sinabek/licences/blob/main/README.md)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/sinabek/licences/blob/main/README.pt.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.es.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.fr.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.de.md)


Wir werden oft gefragt, welche Lizenz wir ihnen für ihr Projekt empfehlen. Wir haben darüber bereits öffentlich geschrieben, die Informationen sind jedoch auf verschiedene Aufsätze, FAQ-Einträge und Lizenzkommentare verstreut. Dieser Artikel fasst alle diese Informationen in einer einzigen Quelle zusammen, um es den Menschen zu erleichtern, ihnen zu folgen und darauf zurückzugreifen.


Diese Empfehlungen gelten für Arbeiten, die für praktische Aufgaben konzipiert sind. Dazu gehören Software, Dokumentation und einige andere Dinge. Kunstwerke und Werke, die einen Standpunkt darlegen, sind unterschiedliche Themen; Das GNU-Projekt hat keinen allgemeinen Standpunkt dazu, wie sie veröffentlicht werden sollten, außer dass sie alle ohne unfreie Software (insbesondere ohne DRM) nutzbar sein sollten. Möglicherweise möchten Sie diese Empfehlungen jedoch für Kunstwerke befolgen, die zu einem bestimmten Programm gehören.


Die Empfehlungen gelten für die Lizenzierung eines von Ihnen erstellten Werks – unabhängig davon, ob es sich um eine Modifikation eines bestehenden Werks oder um ein neues Originalwerk handelt. Sie gehen nicht auf die Frage der Kombination von vorhandenem Material unter verschiedenen Lizenzen ein. Wenn Sie dabei Hilfe suchen, lesen Sie bitte unsere GPL-FAQ.

Nachdem Sie gesehen haben, was wir hier empfehlen, können Sie, wenn Sie Rat wünschen, an <licensing@gnu.org> schreiben. Beachten Sie, dass es wahrscheinlich einige Wochen dauern wird, bis sich das Lizenzierungsteam bei Ihnen meldet. Wenn Sie innerhalb eines Monats keine Antwort erhalten, schreiben Sie uns bitte erneut.


## Beitrag zu einem bestehenden Projekt


Wenn Sie zu einem bestehenden Projekt beitragen, sollten Sie Ihre geänderten Versionen normalerweise unter derselben Lizenz wie das Originalwerk veröffentlichen. Es ist gut, mit den Betreuern des Projekts zusammenzuarbeiten, und die Verwendung einer anderen Lizenz für Ihre Änderungen macht diese Zusammenarbeit oft sehr schwierig. Sie sollten dies nur tun, wenn es einen triftigen Grund dafür gibt.


Ein Fall, in dem die Verwendung einer anderen Lizenz gerechtfertigt sein kann, ist, wenn Sie größere Änderungen an einem Werk unter einer Nicht-Copyleft-Lizenz vornehmen. Wenn die von Ihnen erstellte Version wesentlich nützlicher ist als das Original, lohnt es sich, Ihre Arbeit mit Copyleft zu versehen, und zwar aus den gleichen Gründen, aus denen wir normalerweise Copyleft empfehlen. Wenn Sie sich in dieser Situation befinden, befolgen Sie bitte die folgenden Empfehlungen zur Lizenzierung eines neuen Projekts.


Wenn Sie sich aus irgendeinem Grund dafür entscheiden, Ihre Beiträge unter einer anderen Lizenz zu veröffentlichen, müssen Sie sicherstellen, dass die Originallizenz die Nutzung des Materials unter der von Ihnen gewählten Lizenz erlaubt. Zeigen Sie der Ehrlichkeit halber explizit an, welche Teile des Werkes unter welcher Lizenz stehen.


### Software


Wir empfehlen unterschiedliche Lizenzen für unterschiedliche Projekte, vor allem abhängig vom Einsatzzweck der Software. Im Allgemeinen empfehlen wir die Verwendung der stärksten Copyleft-Lizenz, die diesen Zweck nicht beeinträchtigt. Unser Aufsatz „Was ist Copyleft?“ erklärt das Konzept des Copyleft ausführlicher und warum es im Allgemeinen die beste Lizenzierungsstrategie ist.


Für die meisten Programme empfehlen wir Ihnen, die aktuellste Version der GNU General Public License (GPL) für Ihr Projekt zu verwenden. Sein starkes Copyleft ist für alle Arten von Software geeignet und umfasst zahlreiche Schutzmaßnahmen für die Freiheit der Benutzer. Um zukünftige Lizenz-Upgrades zu ermöglichen, geben Sie bitte „Version 3 oder eine spätere Version“ an, damit Ihr Programm mit Code lizenzkompatibel ist, der möglicherweise in Zukunft unter nachfolgenden GPL-Versionen veröffentlicht wird.


### Kleine Programme


Für die meisten kleinen Programme lohnt es sich nicht, Copyleft zu verwenden. Wir verwenden 300 Zeilen als Maßstab: Wenn der Quellcode eines Softwarepakets kürzer ist, sind die Vorteile von Copyleft in der Regel zu gering, um die Unannehmlichkeiten zu rechtfertigen, sicherzustellen, dass der Software immer eine Kopie der Lizenz beiliegt.


Für diese Programme empfehlen wir die Apache-Lizenz 2.0. Hierbei handelt es sich um eine schwache, laxe „Pushover“-Softwarelizenz (kein Copyleft), deren Bedingungen verhindern sollen, dass Mitwirkende und Distributoren wegen Patentverletzung klagen. Dies macht die Software nicht immun gegen Bedrohungen durch Patente (keine Softwarelizenz kann das erreichen), aber es verhindert, dass Patentinhaber einen „Köder und Schalter“ einrichten, bei dem sie die Software zu kostenlosen Bedingungen veröffentlichen und dann die Zustimmung der Empfänger verlangen unfreie Begriffe in einer Patentlizenz.


Unter den schwachen (Pushover-)Lizenzen ist Apache 2.0 die beste; Wenn Sie also aus irgendeinem Grund eine schwache Lizenz verwenden möchten, empfehlen wir die Verwendung dieser.


### Bibliotheken


Bei Bibliotheken unterscheiden wir drei Arten von Fällen.


Einige Bibliotheken implementieren kostenlose Datenformate, die mit eingeschränkten Datenformaten konkurrieren, wie z. B. Ogg Vorbis (das mit MP3-Audio konkurriert) und WebM (das mit MPEG-4-Video konkurriert). Der Erfolg des freien Formats erfordert die Möglichkeit, dass viele proprietäre Anwendungsprogramme den Code zur Verarbeitung des Formats einbinden können. Wir wollten beispielsweise, dass nicht-freie Mediaplayer, insbesondere Appliances, den Code für Ogg Vorbis sowie MP3 enthalten.


Wenn Sie in diesen besonderen Situationen proprietäre Anwendungsentwickler davon überzeugen möchten, die Bibliothek für das freie Format zu verwenden, müssen Sie dies vereinfachen, indem Sie die Bibliothek unter einer schwachen Lizenz lizenzieren, beispielsweise der Apache-Lizenz 2.0.


Allerdings müssen wir erkennen, dass diese Strategie für Ogg Vorbis keinen Erfolg hatte. Selbst nachdem die Urheberrechtslizenz geändert wurde, um eine einfache Einbindung dieses Bibliothekscodes in proprietäre Anwendungen zu ermöglichen, haben proprietäre Entwickler ihn im Allgemeinen nicht eingebunden. Der Verzicht bei der Wahl der Lizenz hat uns letztlich wenig gebracht.


Für alle anderen Bibliotheken empfehlen wir eine Art Copyleft. Wenn Entwickler bereits eine etablierte alternative Bibliothek verwenden, die unter einer unfreien Lizenz oder einer laxen Pushover-Lizenz veröffentlicht wurde, empfehlen wir die Verwendung der GNU Lesser General Public License (LGPL).


Anders als im ersten Fall, in dem die Bibliothek einen ethisch überlegenen Standard umsetzt, wird hier mit der Übernahme um ihrer selbst willen kein besonderes objektives Ziel erreicht, sodass es keinen Grund gibt, Copyleft gänzlich zu vermeiden. Wenn Sie jedoch von Entwicklern, die Ihre Bibliothek nutzen, verlangen, dass sie ihre gesamten Programme unter Copyleft veröffentlichen, nutzen sie einfach eine der verfügbaren Alternativen, und auch das wird unserer Sache nicht nützen. Die Lesser GPL wurde entwickelt, um den Mittelweg zwischen diesen Fällen zu schließen, indem sie proprietären Softwareentwicklern die Nutzung der abgedeckten Bibliothek ermöglicht, aber ein schwaches Copyleft bietet, das den Benutzern Freiheit hinsichtlich des Bibliothekscodes selbst gibt.


Für Bibliotheken, die spezielle Einrichtungen anbieten und nicht mit fester Konkurrenz ohne Copyleft oder ohne freie Lizenz konfrontiert sind, empfehlen wir die Verwendung der einfachen GNU GPL. Lesen Sie den Artikel „Warum Sie die Lesser GPL nicht für Ihre nächste Bibliothek verwenden sollten“, um die Gründe dafür zu erfahren.


### Serversoftware


Wenn es wahrscheinlich ist, dass andere verbesserte Versionen Ihres Programms für die Ausführung auf Servern erstellen und ihre Versionen nicht an andere weitergeben, und Sie befürchten, dass dadurch Ihre veröffentlichte Version benachteiligt wird, empfehlen wir die GNU Affero General Public License (AGPL). Die Bedingungen der AGPL sind nahezu identisch mit denen der GPL; Der einzige wesentliche Unterschied besteht darin, dass es eine zusätzliche Bedingung gibt, um sicherzustellen, dass Personen, die die Software über ein Netzwerk verwenden, den Quellcode dafür erhalten können.


Die Anforderungen der AGPL gehen nicht auf die Probleme ein, die für Benutzer entstehen können, wenn sie ihre Computer oder Daten dem Server eines anderen anvertrauen. Beispielsweise wird es Service as a Software Substitute (SaaSS) nicht davon abhalten, den Benutzern die Freiheit zu verweigern – aber die meisten Server bieten kein SaaSS an. Weitere Informationen zu diesen Problemen finden Sie unter „Warum die Affero GPL“.


### Dokumentation


Wir empfehlen die GNU Free Documentation License (GFDL) für Tutorials, Referenzhandbücher und andere umfangreiche Dokumentationswerke. Es handelt sich um eine starke Copyleft-Lizenz für Lehrwerke, die ursprünglich für Softwarehandbücher geschrieben wurde und Bedingungen enthält, die speziell auf häufige Probleme eingehen, die bei der Verbreitung oder Änderung dieser Werke auftreten.


Für kurze, sekundäre Dokumentationsarbeiten, beispielsweise eine Referenzkarte, ist es besser, die GNU-All-Permissive-Lizenz zu verwenden, da eine Kopie der GFDL kaum in eine Referenzkarte passen würde. Verwenden Sie nicht CC BY, da es mit der GFDL nicht kompatibel ist.


Für Manpages empfehlen wir die GFDL, wenn die Seite lang ist, und die GNU-All-Permissive-Lizenz, wenn sie kurz ist.


Einige Dokumentationen enthalten Software-Quellcode. Beispielsweise könnte ein Handbuch für eine Programmiersprache Beispiele enthalten, denen die Leser folgen können. Sie sollten diese sowohl gemäß den FDL-Bedingungen in das Handbuch aufnehmen als auch unter einer anderen, für Software geeigneten Lizenz veröffentlichen. Dies erleichtert die Verwendung des Codes in anderen Projekten. Wir empfehlen, dass Sie kleine Teile des Codes mithilfe von CC0 öffentlich zugänglich machen und größere Teile unter derselben Lizenz verteilen, die das zugehörige Softwareprojekt verwendet.


### Weitere Daten zu Programmen


In diesem Abschnitt werden alle anderen Werke für den praktischen Gebrauch besprochen, die Sie möglicherweise in die Software einbinden. Dazu gehören beispielsweise Symbole und andere funktionale oder nützliche Grafiken, Schriftarten und geografische Daten. Sie können ihnen auch für Kunst folgen, obwohl wir es nicht kritisieren würden, wenn Sie dies nicht tun.


Wenn Sie diese Werke speziell für die Verwendung in einem Softwareprojekt erstellen, empfehlen wir Ihnen grundsätzlich, Ihre Arbeit unter derselben Lizenz wie die Software zu veröffentlichen. Mit den von uns empfohlenen Lizenzen ist dies kein Problem: GPLv3, LGPLv3, AGPLv3 und GPLv2 können alle auf jede Art von Werk – nicht nur auf Software – angewendet werden, das urheberrechtlich geschützt ist und eine klare bevorzugte Form für die Änderung hat. Die Verwendung derselben Lizenz wie die Software trägt dazu bei, die Compliance für Händler zu erleichtern und jeden Zweifel über mögliche Kompatibilitätsprobleme zu vermeiden. Die Verwendung einer anderen kostenlosen Lizenz kann sinnvoll sein, wenn sie einen konkreten praktischen Nutzen bietet, beispielsweise eine bessere Zusammenarbeit mit anderen kostenlosen Projekten.


Wenn Ihre Arbeit nicht für die Verwendung mit einem bestimmten Softwareprojekt erstellt wird oder wenn es nicht angemessen wäre, dieselbe Lizenz wie das Projekt zu verwenden, empfehlen wir Ihnen lediglich, eine Copyleft-Lizenz zu wählen, die für Ihre Arbeit geeignet ist. Einige davon sind in unserer Lizenzliste aufgeführt. Wenn keine Lizenz besonders geeignet erscheint, ist die Creative Commons Attribution-ShareAlike-Lizenz ein Copyleft, das für viele verschiedene Arten von Werken verwendet werden kann.