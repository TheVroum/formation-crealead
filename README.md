Liste des points à respecter pour être au standard d'accessibilité RGAA 3, pour le Gabarit Général et la Navigation :



1.

[ ] doctype valide au début

[ ] document validé (exempt d'erreurs, pas forcément sans warnings)

[ ] banner sur le header principal, de même contentinfo pour le footer principal, main pour le main, un ou plusieurs navigation pour les navs principales

[ ] un search pour la barre de recherche du site

[ ] RGAA insiste sur le fait de doubler même les balises sémantiques par les rôles aria

[ ] ils conseillent de ne pas imbriquer les régions définies ici, c'est à dire qu'aucune d'entre elle ne doit pas être fille l'une d'une autre



2.

[ ] concernant les systèmes de navigation dans le site, il doit y en avoir au moins deux. Si je devais résumer le paragraphe, je dirais que c'est par ce qu'aucun ne couvrira la totalité des utilisateurs. Mais si un système en laisse de côté 1/2, alors 2 en laisseront 1/4.

[ ] ne concernent pas les site avec 2 ou 3 pages pour lesquels un menu de navigation suffit, et les monopages, pour les liens d'accès rapide détaillés juste après suffisent, associé au ctrl + f.

[ ] pour aider particulièrement les utilisateurs sans souris, utiliser un liens d'accès rapide vers le contenu, ou le tabindex pour accéder par exemple à un champ de recherche ou textuel.

[ ] fournir aussi des liens pour accéder aux groupes de liens importants

[ ] lorsqu'on met en place des balises pour l'accessibilité, ne pas utiliser les propriétés/attributs suivants, dans l'éventualité on souhaite les masquer aux autres utilisateurs par exemple ou pour tout autre raison : css[display none, visibility hidden, width/height 0, fontsize 0], et en html[hidden, et aria-hidden="true" ou en booléen aussi j'imagine]

[ ] ces éléments d'accessibilité pour être efficaces doivent être au début du code et de la page, et ils conseillent d'en faire les premiers liens.

[ ] ils doivent être dans le même ordre. En cas d'élément éventuel ? Je comprends que s'ils ne sont pas statiques, ils doivent être déterministes et ne pas changer d'ordre pour rien, au gré des aléas du code. J'aurais utilisé le mot constance et prévisibilité. Ils utilisent le mot cohérent.

[ ] Il y a le moteur de recherche (inerne ici, ou tout du moins, pour le site), et la navigation prncipale.

[ ] Le plan du site. Verifier que les liens fonctionnent.

[ ] prêter une attention particulière à la balise titre, qui est souvent vocalisé et est un repère pour beaucoup d'utilisateur (aacessibilité, ainsi que ceux qui utilisent l'historique ou beaucoup d'onglets)

[ ] pour les pages dynamiques : pour les recherche, indiquer la pagination, si on est issu d'un formulaire et qu'on a eu des erreurs en retour, le mentionner dans le titre.

[ ] les collections de pages (par exemple partie contenant des chapitres d'un cours) doivent avoir l'aria navigation, et éventuellement un aria label pour les distinguer. Ils conseillent de mettre des liens vers précédent, précédent, et tout, depuis chaque page, ce qui peut être facile, difficile, ou impossible s'il s'agit de site externe.

[ ] dans "le" menu de navigation, ils conseillent de marquer la page courante, pour ce faire, en plus par exemple de couleur, ils conseillent d'ajouter au texte "en cours de consultation".

[ ] ils conseillent de combiner les méthodes pour couvrir le maximum d'utilsateur : couleur de fond, forme/icône adjacente, ajouter un title sur le liens de la page courante (pour les problèmes de visions, ou les feuilles de style utilisateur). Moi : laisser cliquable ? On risque des fois, si la page a un gros pattern, de ne même pas se rendre compte qu'il s'agit de la même page rafraichie.

[ ] 2 fil d'ariane : système de navigation reconnu. Faire figurer la page dans l'arborescence du site.
