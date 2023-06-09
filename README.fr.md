# How to Choose a License for Your Own Work
[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/sinabek/licences/blob/main/README.md)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/sinabek/licences/blob/main/README.pt.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.es.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.fr.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.de.md)


Les gens nous demandent souvent quelle licence nous leur recommandons d'utiliser pour leur projet. Nous avons déjà écrit publiquement à ce sujet, mais les informations ont été éparpillées entre différents essais, entrées de FAQ et commentaires de licence. Cet article rassemble toutes ces informations dans une source unique, pour faciliter le suivi et la référence.


Ces recommandations s'appliquent aux travaux conçus pour effectuer des travaux pratiques. Ceux-ci incluent des logiciels, de la documentation et d'autres choses. Les œuvres d'art et les œuvres qui expriment un point de vue sont des questions différentes; le projet GNU n'a pas de position générale sur la façon dont ils devraient être publiés, sauf qu'ils devraient tous être utilisables sans logiciel non libre (en particulier, sans DRM). Cependant, vous voudrez peut-être suivre ces recommandations pour les œuvres d'art qui accompagnent un programme particulier.


Les recommandations s'appliquent à la licence d'une œuvre que vous créez, qu'il s'agisse d'une modification d'une œuvre existante ou d'une nouvelle œuvre originale. Ils n'abordent pas la question de la combinaison de matériel existant sous différentes licences. Si vous cherchez de l'aide à ce sujet, veuillez consulter notre FAQ GPL.

Après avoir vu ce que nous recommandons ici, si vous souhaitez des conseils, vous pouvez écrire à <licensing@gnu.org>. Notez qu'il faudra probablement quelques semaines à l'équipe des licences pour vous répondre ; si vous n'obtenez pas de réponse dans un mois, veuillez réécrire.


## Contribuer à un projet existant


Lorsque vous contribuez à un projet existant, vous devez généralement publier vos versions modifiées sous la même licence que l'œuvre originale. Il est bon de coopérer avec les mainteneurs du projet, et l'utilisation d'une licence différente pour vos modifications rend souvent cette coopération très difficile. Vous ne devriez le faire que lorsqu'il y a une bonne raison de le justifier.


Un cas où l'utilisation d'une licence différente peut être justifiée est lorsque vous apportez des modifications majeures à une œuvre sous une licence non-copyleft. Si la version que vous avez créée est considérablement plus utile que l'original, alors cela vaut la peine de copier votre travail, pour toutes les mêmes raisons que nous recommandons normalement. Si vous êtes dans cette situation, veuillez suivre les recommandations ci-dessous pour autoriser un nouveau projet.


Si vous choisissez de publier vos contributions sous une licence différente pour quelque raison que ce soit, vous devez vous assurer que la licence d'origine autorise l'utilisation du matériel sous la licence choisie. Par souci d'honnêteté, indiquez explicitement quelles parties de l'œuvre sont sous quelle licence.


### Logiciel


Nous recommandons différentes licences pour différents projets, en fonction principalement de l'objectif du logiciel. En général, nous recommandons d'utiliser la licence de copyleft la plus forte qui n'interfère pas avec cet objectif. Notre essai « Qu'est-ce que le copyleft ? » explique le concept de copyleft plus en détail, et pourquoi c'est généralement la meilleure stratégie de licence.


Pour la plupart des programmes, nous vous recommandons d'utiliser la version la plus récente de la licence publique générale GNU (GPL) pour votre projet. Son fort copyleft convient à tous les types de logiciels et inclut de nombreuses protections pour la liberté des utilisateurs. Pour permettre de futures mises à niveau de licence, veuillez spécifier "version 3 ou toute version ultérieure" afin que votre programme soit compatible avec la licence du code qui pourrait être publié, à l'avenir, sous des versions GPL ultérieures.


### Petits programmes


Cela ne vaut pas la peine d'utiliser le copyleft pour la plupart des petits programmes. Nous utilisons 300 lignes comme référence : lorsque le code source d'un progiciel est plus court que cela, les avantages fournis par le copyleft sont généralement trop faibles pour justifier l'inconvénient de s'assurer qu'une copie de la licence accompagne toujours le logiciel.


Pour ces programmes, nous recommandons la licence Apache 2.0. Il s'agit d'une licence de logiciel faible, laxiste, "pushover" (non-copyleft) qui a des termes pour empêcher les contributeurs et les distributeurs de poursuivre en justice pour contrefaçon de brevet. Cela ne rend pas le logiciel à l'abri des menaces de brevets (aucune licence de logiciel ne peut y parvenir), mais cela empêche les titulaires de brevets de mettre en place un «appât et un commutateur» où ils publient le logiciel sous des conditions gratuites, puis exigent que les destinataires acceptent de termes non libres dans une licence de brevet.


Parmi les licences faibles (pushover), Apache 2.0 est la meilleure ; donc si vous allez utiliser une licence faible, quelle qu'en soit la raison, nous vous recommandons d'utiliser celle-ci.


### Bibliothèques


Pour les bibliothèques, on distingue trois types de cas.


Certaines bibliothèques implémentent des formats de données libres qui sont en concurrence avec des formats de données restreints, tels que Ogg Vorbis (qui concurrence l'audio MP3) et WebM (qui concurrence la vidéo MPEG-4). Le succès du format libre nécessite de permettre à de nombreux programmes d'application propriétaires de se lier au code pour gérer le format. Par exemple, nous voulions que les lecteurs multimédias non libres, en particulier les appareils, incluent le code pour Ogg Vorbis ainsi que MP3.


Dans ces situations particulières, si vous souhaitez convaincre les développeurs d'applications propriétaires d'utiliser la bibliothèque pour le format libre, vous devrez faciliter cela en attribuant à la bibliothèque une licence faible, telle que la licence Apache 2.0.


Cependant, force est de reconnaître que cette stratégie n'a pas réussi pour Ogg Vorbis. Même après avoir modifié la licence de copyright pour permettre l'inclusion facile de ce code de bibliothèque dans des applications propriétaires, les développeurs propriétaires ne l'ont généralement pas inclus. Le sacrifice consenti dans le choix de la licence nous a finalement peu gagné.


Pour toutes les autres bibliothèques, nous recommandons une sorte de copyleft. Si les développeurs utilisent déjà une bibliothèque alternative établie publiée sous une licence non libre ou une licence pushover laxiste, nous vous recommandons d'utiliser la licence publique générale limitée GNU (LGPL).


Contrairement au premier cas, où la bibliothèque met en œuvre une norme éthiquement supérieure, ici l'adoption pour elle-même n'accomplira aucun objectif objectif particulier, il n'y a donc aucune raison d'éviter complètement le copyleft. Cependant, si vous demandez aux développeurs qui utilisent votre bibliothèque de publier leurs programmes entiers sous copyleft, ils utiliseront simplement l'une des alternatives disponibles, et cela ne fera pas non plus avancer notre cause. La Lesser GPL a été conçue pour combler le juste milieu entre ces cas, permettant aux développeurs de logiciels propriétaires d'utiliser la bibliothèque couverte, mais fournissant un copyleft faible qui donne aux utilisateurs la liberté concernant le code de la bibliothèque lui-même.


Pour les bibliothèques qui fournissent des installations spécialisées et qui ne sont pas confrontées à une concurrence non copyleftée ou non libre, nous recommandons d'utiliser la GNU GPL ordinaire. Pour les raisons, lisez "Pourquoi vous ne devriez pas utiliser la Lesser GPL pour votre prochaine bibliothèque".


### Logiciel serveur


S'il est probable que d'autres créeront des versions améliorées de votre programme pour qu'elles s'exécutent sur des serveurs et ne distribuent leurs versions à personne d'autre, et que vous craignez que cela ne désavantage votre version publiée, nous vous recommandons la licence publique générale GNU Affero. (AGPL). Les termes de l'AGPL sont presque identiques à ceux de la GPL ; la seule différence substantielle est qu'il a une condition supplémentaire pour s'assurer que les personnes qui utilisent le logiciel sur un réseau pourront obtenir le code source pour celui-ci.


L'exigence de l'AGPL ne résout pas les problèmes qui peuvent survenir pour les utilisateurs lorsqu'ils confient leur informatique ou leurs données au serveur de quelqu'un d'autre. Par exemple, cela n'empêchera pas le service en tant que substitut de logiciel (SaaSS) de nier la liberté des utilisateurs, mais la plupart des serveurs ne font pas de SaaSS. Pour en savoir plus sur ces problèmes, lisez "Pourquoi l'Affero GPL".


### Documentation


Nous recommandons la licence de documentation gratuite GNU (GFDL) pour les didacticiels, les manuels de référence et d'autres gros travaux de documentation. Il s'agit d'une licence de copyleft forte pour les travaux éducatifs, initialement écrite pour les manuels de logiciels, et comprend des termes qui traitent spécifiquement des problèmes courants qui surviennent lorsque ces travaux sont distribués ou modifiés.


Pour les travaux de documentation courts et secondaires, comme une carte de référence, il est préférable d'utiliser la licence tout permissive GNU, car une copie de la GFDL pourrait difficilement tenir dans une carte de référence. N'utilisez pas CC BY, car il est incompatible avec la GFDL.


Pour les pages de manuel, nous recommandons la GFDL si la page est longue et la licence GNU tout permis si elle est courte.


Certaines documentations incluent le code source du logiciel. Par exemple, un manuel pour un langage de programmation peut inclure des exemples à suivre par les lecteurs. Vous devez à la fois les inclure dans le manuel selon les termes de la FDL et les publier sous une autre licence appropriée pour le logiciel. Cela facilite l'utilisation du code dans d'autres projets. Nous vous recommandons de dédier de petits morceaux de code au domaine public à l'aide de CC0 et de distribuer des morceaux plus volumineux sous la même licence que celle utilisée par le projet logiciel associé.


### Autres données pour les programmes


Cette section traite de tous les autres travaux à usage pratique que vous pourriez inclure avec le logiciel. Pour vous donner quelques exemples, cela inclut les icônes et autres graphiques, polices et données géographiques fonctionnels ou utiles. Vous pouvez également les suivre pour l'art, même si nous ne critiquerions pas si vous ne le faites pas.


Si vous créez ces travaux spécifiquement pour une utilisation avec un projet logiciel, nous vous recommandons généralement de publier votre travail sous la même licence que le logiciel. Il n'y a aucun problème à le faire avec les licences que nous avons recommandées : GPLv3, LGPLv3, AGPLv3 et GPLv2 peuvent toutes être appliquées à n'importe quel type de travail - pas seulement un logiciel - qui est protégé par le droit d'auteur et a une forme préférée claire pour la modification. L'utilisation de la même licence que le logiciel facilitera la conformité pour les distributeurs et évitera tout doute sur les problèmes de compatibilité potentiels. L'utilisation d'une licence libre différente peut être appropriée si elle offre un avantage pratique spécifique, comme une meilleure coopération avec d'autres projets libres.


Si votre travail n'est pas créé pour être utilisé avec un projet logiciel particulier, ou s'il ne serait pas approprié d'utiliser la même licence que le projet, nous vous recommandons uniquement de choisir une licence copyleft appropriée pour votre travail. Certains d'entre eux figurent sur notre liste de licences. Si aucune licence ne semble particulièrement appropriée, la licence Creative Commons Attribution-ShareAlike est un copyleft qui peut être utilisé pour de nombreux types d'œuvres.