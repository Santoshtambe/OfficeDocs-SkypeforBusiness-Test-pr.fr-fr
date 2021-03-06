﻿---
title: 'Lync Server 2013 : Rapport de synthèse de la qualité des médias'
TOCTitle: Rapport de synthèse de la qualité des médias
ms:assetid: 8bd59ad6-3087-49c8-b692-5573fe2ffcd8
ms:mtpsurl: https://technet.microsoft.com/fr-fr/library/Gg615012(v=OCS.15)
ms:contentKeyID: 49297999
ms.date: 07/01/2016
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Rapport de synthèse de la qualité des médias dans Lync Server 2013

 

_**Dernière rubrique modifiée :** 2016-06-29_

Le rapport de synthèse de la qualité des médias permet d’analyser la qualité des appels au sein de votre organisation : ce rapport fournit des mesures d’appel de qualité de l’expérience (QoE) détaillées décomposées selon les catégories suivantes :

  - Appels P2P UC (par exemple, un appel Microsoft Lync 2013 vers Microsoft Lync 2013)

  - Sessions de conférence UC

  - Sessions de conférence RTC

  - Appels RTC : contournement du média

  - Appels RTC (sans contournement) : partie UC

  - Appels RTC (sans contournement) : partie passerelle

  - Autres types d’appels

Quand vous ouvrez le rapport pour la première fois, une synthèse des informations pour chaque catégorie s’affiche. Sans quitter le rapport, vous pouvez développer chaque catégorie pour afficher des sous-catégories, telles que les appels passés de Office Communicator 2007 R2 vers Lync 2013. Vous pouvez développer également ces sous-catégories pour afficher des détails sur chaque appel passé dans cette sous-catégorie.

Dans Microsoft Lync Server 2013, le rapport de synthèse de la qualité des médias décompose les données en trois types d’appel : appels audio, appels vidéo et appels de partage d’application. Chaque type d’appel correspond à une section du rapport, et dispose d’un ensemble personnalisé de mesures des appels.

Le rapport de synthèse de la qualité des médias vous permet d’appliquer des filtres pour comparer la qualité des appels entre les appels câblés et les appels sans fil, les appels internes et externes, les appels VPN et non VPN.

## Accès au rapport de synthèse de la qualité des médias

Le rapport de synthèse de la qualité des médias est accessible à partir de la page d’accueil Rapports de surveillance. Vous pouvez accéder au [Rapport de la liste d’appels dans Lync Server 2013](lync-server-2013-call-list-report.md) en cliquant sur l’une des mesures suivantes :

  - Volume d’appels

  - Pourcentage d’appels médiocres

De plus, vous pouvez accéder au Rapport de distribution des mesures de qualité des médias en cliquant sur l’une des mesures d’appel audio suivantes :

  - Boucle (ms)

  - Dégradation (MOS)

  - Perte de paquets

  - Gigue (ms)

  - Taux de masquage de la réparation

  - Taux d’étirement de la réparation

  - Taux de compression de la réparation

## Filtres

Les filtres vous offrent la possibilité de renvoyer un ensemble de données mieux ciblées ou de visualiser les données renvoyées de différentes manières. Par exemple, grâce au rapport de synthèse de la qualité des médias, vous pouvez filtrer les données renvoyées selon des éléments précis, tels que le type d’accès (à savoir « accès interne » par comparaison à « accès externe ») ou la connexion réseau câblée/sans fil. Vous pouvez également choisir le mode de groupement des données. Dans ce cas, les appels sont groupés par heure, jour, semaine ou mois.

Le tableau qui suit dresse la liste des filtres que vous pouvez utiliser avec le rapport de synthèse de la qualité des médias.

### Filtres du rapport de synthèse de la qualité des médias

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Nom</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>De</strong></p></td>
<td><p>Date/heure de début de la période. Pour afficher les données par heures, entrez à la fois la date et l’heure de début comme suit :</p>
<p>7/7/2012 1:00 PM</p>
<p>Si vous ne précisez aucune heure de début, le rapport commence automatiquement à midi (12:00 AM) à la date du jour défini. Pour afficher les données par jour, entrez simplement la date :</p>
<p>7/7/2012</p>
<p>Pour afficher les données par semaine ou mois, entrez une date tombant un jour quelconque de la semaine ou du mois que vous souhaitez visualiser (nul besoin d’entrer le premier jour de la semaine ou du mois) :</p>
<p>7/3/2012</p>
<p>Les semaines s’étalent toujours du dimanche au samedi.</p></td>
</tr>
<tr class="even">
<td><p><strong>À</strong></p></td>
<td><p>Date/heure de fin de la période. Pour afficher les données par heures, entrez à la fois la date et l’heure de fin comme suit :</p>
<p>7/7/2012 1:00 PM</p>
<p>Si vous ne précisez aucune heure de fin, le rapport se termine automatiquement à midi (12:00 AM) à la date du jour défini. Pour afficher les données par jour, entrez simplement la date :</p>
<p>7/7/2012</p>
<p>Pour afficher les données par semaine ou mois, entrez une date tombant un jour quelconque de la semaine ou du mois que vous souhaitez visualiser (nul besoin d’entrer le premier jour de la semaine ou du mois) :</p>
<p>7/3/2012</p>
<p>Les semaines s’étalent toujours du dimanche au samedi.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type d’accès</strong></p></td>
<td><p>Indique si le client était connecté au réseau interne ou au réseau externe au moment de passer l’appel. Sélectionnez l’une des options suivantes :</p>
<ul>
<li><p>[Tous]</p></li>
<li><p>Interne</p></li>
<li><p>Externe</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Type de réseau</strong></p></td>
<td><p>Indique le type de réseau auquel le client était connecté au moment où l’appel a été émis. Sélectionnez l’une des options suivantes :</p>
<ul>
<li><p>[Tous]</p></li>
<li><p>Câblé</p></li>
<li><p>Sans fil</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>VPN</strong></p></td>
<td><p>Indique si un client externe utilisait une connexion de réseau privé virtuel (VPN) au moment d’effectuer l’appel. Sélectionnez l’une des options suivantes :</p>
<ul>
<li><p>[Tous]</p></li>
<li><p>VPN</p></li>
<li><p>Non-VPN</p></li>
</ul></td>
</tr>
</tbody>
</table>


## Mesures

Le tableau qui suit répertorie les informations fournies dans le rapport de synthèse de la qualité des médias.

### Mesures du rapport de synthèse de la qualité des médias : synthèse des appels audio

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nom</th>
<th>Est-il possible d’effectuer un tri sur cet élément ?</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Type d’appel/type de point de terminaison</strong></p></td>
<td><p>Non</p></td>
<td><p>Lorsque vous cliquez sur cet élément, le rapport affiche des informations détaillées sur les appels en fonction de ce type. Les types d’appels sont les suivants :</p>
<ul>
<li><p>Appels P2P UC</p></li>
<li><p>Sessions de conférence UC</p></li>
<li><p>Sessions de conférence RTC</p></li>
<li><p>Appels RTC : contournement du média</p></li>
<li><p>Appels RTC (sans contournement) : partie UC</p></li>
<li><p>Appels RTC (sans contournement) : partie passerelle</p></li>
<li><p>Autres types d’appels</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels par type d’appel.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Pourcentage d’appels médiocres</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels jugés et classés comme étant médiocres. Un appel médiocre désigne un appel dont l’une des valeurs mesurées est supérieure à la valeur autorisée (par exemple, un appel soumis à un phénomène de gigue excessive).</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels (appels sans fil)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels qui utilisaient une connexion sans fil.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Volume d’appels (appels VPN)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels qui utilisaient une connexion VPN.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels (appels externes)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre d’appels qui utilisaient une connexion externe (c’est-à-dire une connexion en dehors du réseau interne).</p></td>
</tr>
<tr class="odd">
<td><p><strong>Boucle (ms)</strong></p></td>
<td><p>Non</p></td>
<td><p>Temps moyen (en millisecondes) nécessaire à un package RTP (Real-Time Transport Protocol) pour effectuer un aller-retour vers un autre point de terminaison. Des boucles de 100 millisecondes ou moins sont considérées qualitativement acceptables.</p>
<p>Des boucles avec des temps plus élevés peuvent être causées par le routage international des appels, une mauvaise configuration du routage ou un serveur multimédia surchargé. Les temps d’aller-retour élevés créent des difficultés dans le cadre de conversations audio bidirectionnelles réalisées en temps réel.</p></td>
</tr>
<tr class="even">
<td><p><strong>Dégradation (MOS)</strong></p></td>
<td><p>Non</p></td>
<td><p>Taux moyen de dégradation de la note moyenne d’opinion (MOS) observé au cours d’un appel. Les valeurs de dégradation peuvent aller de 0,0 (la plus faible) à 5,0 (la plus élevée). Une valeur de 0,5 ou moins signifie une dégradation acceptable. Traditionnellement, les notes moyennes d’opinion sont calculées en demandant aux utilisateurs d’évaluer la qualité d’un appel sur une échelle de 1 à 5. Dans Lync Server, Lync Server se sert d’un ensemble d’algorithmes pour prédire la manière dont les utilisateurs auraient évalué un appel.</p>
<p>Les valeurs de dégradation élevées peuvent provenir d’une congestion, d’un dépassement de la bande passante disponible, d’une congestion/interférence dans la liaison sans fil ou bien d’un serveur multimédia ou d’un point de terminaison surchargé, ce qui se traduit par une distorsion ou une perte de l’audio.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Perte de paquets</strong></p></td>
<td><p>Non</p></td>
<td><p>Taux moyen de pertes de paquets RTP. (La perte de paquets survient lorsque des paquets RTP, protocole employé pour la transmission audio et vidéo sur Internet, n’atteignent pas leur point de destination.) Les valeurs de perte élevées peuvent provenir d’une congestion, d’un dépassement de la bande passante disponible, d’une congestion/interférence dans la liaison sans fil ou d’un serveur multimédia surchargé, ce qui se traduit par une distorsion ou une perte de l’audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>Gigue (ms)</strong></p></td>
<td><p>Non</p></td>
<td><p>Gigue moyenne détectée entre les arrivées de paquets RTP. (La gigue permet de mesurer les fluctuations d’un appel.) Les valeurs de gigue élevées peuvent provenir d’une congestion ou d’un serveur multimédia surchargé, ce qui se traduit par une distorsion ou une perte de l’audio.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Taux de masquage de la réparation</strong></p></td>
<td><p>Non</p></td>
<td><p>Ratio moyen d’échantillons audio masqués par rapport au nombre total d’échantillons. (Un échantillon audio masqué est une technique employée pour adoucir les effets de transition violents généralement causés par des paquets réseau perdus.) Des valeurs élevées indiquent des niveaux importants de masquage des pertes appliqués suite à la perte de paquets ou des phénomènes de gigue. Elles se traduisent par une distorsion ou une perte de l’audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>Taux d’étirement de la réparation</strong></p></td>
<td><p>Non</p></td>
<td><p>Ratio moyen d’échantillons audio étirés par rapport au nombre total d’échantillons. (Un échantillon audio étiré est un composant audio qui a été étendu dans le but de maintenir la qualité des appels lorsqu’un paquet réseau perdu est détecté.) Les valeurs élevées indiquent l’existence de niveaux importants d’étirement d’échantillons dus au phénomène de gigue, ce qui se traduit par un effet de robotisation ou de distorsion de l’audio.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Taux de compression de la réparation</strong></p></td>
<td><p>Non</p></td>
<td><p>Ratio moyen d’échantillons audio compressés par rapport au nombre total d’échantillons. (Un échantillon audio compressé est un composant audio qui a été compressé dans le but de maintenir la qualité des appels lorsqu’un paquet réseau perdu est détecté.) Les valeurs élevées indiquent l’existence de niveaux importants de compression d’échantillons dus au phénomène de gigue, ce qui se traduit par un effet d’accélération ou de distorsion de l’audio.</p></td>
</tr>
</tbody>
</table>


### Mesures du rapport de synthèse de la qualité des médias : synthèse des appels vidéo

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nom</th>
<th>Est-il possible d’effectuer un tri sur cet élément ?</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Type d’appel/type de point de terminaison</strong></p></td>
<td><p>Non</p></td>
<td><p>Lorsque vous cliquez sur cet élément, le rapport affiche des informations détaillées sur les appels en fonction de ce type. Les types d’appels sont les suivants :</p>
<ul>
<li><p>Appels P2P UC</p></li>
<li><p>Sessions de conférence UC</p></li>
<li><p>Sessions de conférence RTC</p></li>
<li><p>Appels RTC : contournement du média</p></li>
<li><p>Appels RTC (sans contournement) : partie UC</p></li>
<li><p>Appels RTC (sans contournement) : partie passerelle</p></li>
<li><p>Autres types d’appels</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels par type d’appel.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Pourcentage d’appels médiocres</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels jugés et classés comme étant médiocres. Un appel médiocre désigne un appel dont l’une des valeurs mesurées est supérieure à la valeur autorisée (par exemple, un appel soumis à un phénomène de gigue excessive).</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels (appels sans fil)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels qui utilisaient une connexion sans fil.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Volume d’appels (appels VPN)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels qui utilisaient une connexion VPN.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels (appels externes)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre d’appels qui utilisaient une connexion externe (c’est-à-dire une connexion en dehors du réseau interne).</p></td>
</tr>
<tr class="odd">
<td><p><strong>Vitesse de transmission moyenne (Kbit/s)</strong></p></td>
<td><p>Non</p></td>
<td><p>Vitesse de transmission vidéo moyenne (en kilobits par seconde).</p></td>
</tr>
<tr class="even">
<td><p><strong>Vitesse de transmission faible (%)</strong></p></td>
<td><p>Non</p></td>
<td><p>Pourcentage de l’appel où la vitesse de transmission était faible.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Perte de paquets sortante</strong></p></td>
<td><p>Non</p></td>
<td><p>Perte de paquets RTP (Real-Time Transport Protocol) pour les paquets sortants. (La perte de paquets survient lorsque des paquets RTP, protocole employé pour la transmission audio et vidéo sur Internet, n’atteignent pas leur point de destination.) Les valeurs de perte élevées peuvent provenir d’une congestion, d’un dépassement de la bande passante disponible, d’une congestion/interférence dans la liaison sans fil ou d’un serveur multimédia surchargé, ce qui se traduit par une distorsion ou une perte de l’audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>Image figée (%)</strong></p></td>
<td><p>Non</p></td>
<td><p>Pourcentage d’images « figées ». Dans une image figée, la vidéo cesse d’avancer tandis que la partie audio de l’appel continue.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Fréquence d’images moyenne sortante</strong></p></td>
<td><p>Non</p></td>
<td><p>Fréquence d’images moyenne pour les transmissions sortantes pendant l’appel.</p></td>
</tr>
<tr class="even">
<td><p><strong>Fréquence d’images moyenne entrante</strong></p></td>
<td><p>Non</p></td>
<td><p>Fréquence d’images moyenne pour les transmissions entrantes pendant l’appel.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Fréquence d’images basse entrante (%)</strong></p></td>
<td><p>Non</p></td>
<td><p>Pourcentage de l’appel où la vitesse de transmission pour la vidéo entrante était faible.</p></td>
</tr>
<tr class="even">
<td><p><strong>Intégrité des clients (%)</strong></p></td>
<td><p></p></td>
<td><p>Indique l’intégrité relative du périphérique client pendant l’appel.</p></td>
</tr>
</tbody>
</table>


### Mesures du rapport de synthèse de la qualité des médias : synthèse des appels de partage d’application

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nom</th>
<th>Est-il possible d’effectuer un tri sur cet élément ?</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Type d’appel/type de point de terminaison</strong></p></td>
<td><p>Non</p></td>
<td><p>Lorsque vous cliquez sur cet élément, le rapport affiche des informations détaillées sur les appels en fonction de ce type. Les types d’appels sont les suivants :</p>
<ul>
<li><p>Appels P2P UC</p></li>
<li><p>Sessions de conférence UC</p></li>
<li><p>Sessions de conférence RTC</p></li>
<li><p>Appels RTC : contournement du média</p></li>
<li><p>Appels RTC (sans contournement) : partie UC</p></li>
<li><p>Appels RTC (sans contournement) : partie passerelle</p></li>
<li><p>Autres types d’appels</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels par type d’appel.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Pourcentage d’appels médiocres</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels jugés et classés comme étant médiocres. Un appel médiocre désigne un appel dont l’une des valeurs mesurées est supérieure à la valeur autorisée (par exemple, un appel soumis à un phénomène de gigue excessive).</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels (appels sans fil)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels qui utilisaient une connexion sans fil.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Volume d’appels (appels VPN)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre total d’appels qui utilisaient une connexion VPN.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume d’appels (appels externes)</strong></p></td>
<td><p>Non</p></td>
<td><p>Nombre d’appels qui utilisaient une connexion externe (c’est-à-dire une connexion en dehors du réseau interne).</p></td>
</tr>
<tr class="odd">
<td><p><strong>Gigue (ms)</strong></p></td>
<td><p>Non</p></td>
<td><p>Gigue moyenne détectée entre les arrivées de paquets RTP. (La gigue permet de mesurer les fluctuations d’un appel.) Les valeurs de gigue élevées peuvent provenir d’une congestion ou d’un serveur multimédia surchargé, ce qui se traduit par une distorsion ou une perte de l’audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>Unilatéral relatif moyen</strong></p></td>
<td><p>Non</p></td>
<td><p>Retard unilatéral relatif moyen entre deux points de terminaison du média. Il s’agit d’une mesure de latence sur un seul tronçon.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Latence moyenne de traitement des mosaïques RDP</strong></p></td>
<td><p>Non</p></td>
<td><p>Latence moyenne de traitement des mosaïques RDP sur le serveur de conférence AS par rapport à la durée de la session de visionnage. Cette mesure ne couvre pas la latence du réseau. Une moyenne élevée indique un délai plus long pour l’expérience de visionnage. Un serveur de conférence surchargé peut rencontrer des délais moyens plus élevés.</p></td>
</tr>
<tr class="even">
<td><p><strong>Nombre total de mosaïques altérées (%)</strong></p></td>
<td><p>Non</p></td>
<td><p>Pourcentage total de mosaïques RDP altérées.</p></td>
</tr>
</tbody>
</table>

