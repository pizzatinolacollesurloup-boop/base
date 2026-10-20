# Protocole du relais documentaire

## Circuit minimum

1. Codex lit l'état courant et identifie le manque précis.
2. Il prépare une demande publique neutre `DOC-NNN`, sans pièce ni référence privée. Le détail sensible nécessaire reste dans un brief privé.
3. Le titulaire transmet à Work la demande et, séparément, le lot privé nécessaire.
4. Work vérifie ses outils réels, effectue les seules opérations autorisées et retourne ses résultats détaillés par le canal privé.
5. Le titulaire rapporte ce retour dans la conversation Codex. Codex vérifie les éléments accessibles, puis reprend la mission dépendante.
6. Un compte rendu non sensible peut être enregistré dans GitHub. La demande et l'index sont actualisés sans dupliquer les preuves privées.

L'ouverture de Work et le retour vers Codex sont manuels tant qu'un autre mécanisme n'a pas été établi. Ce protocole ne donne pas de nouvel accès à Drive et ne suppose pas d'API de communication entre conversations.

## Ce qui constitue une preuve

| Observation | Conclusion possible | Limite |
|---|---|---|
| Fichier présent dans le checkout | Préparation locale | Pas de publication GitHub démontrée |
| Commit retrouvé sur le distant | Publication Git vérifiée | Aucun envoi à Work démontré |
| Le titulaire indique avoir transmis à Work | Transmission déclarée par le titulaire | Pas de résultat exécutant reçu |
| Rapport Work avec références et opérations observées | Contrôle rapporté par Work | Pas de lecture Drive directe par Codex si le connecteur manque |
| Copie retournée, ouverte et comparée ici | Contrôle local de la copie reçue | Pas de preuve de l'état actuel de Drive par cette seule copie |
| Réouverture de la source dans Drive par un outil disponible | Vérification directe de cette opération | Ne démontre pas les permissions des autres environnements |

Ne pas publier dans ce tableau de suivi les références privées utilisées pour les contrôles. Le compte rendu public indique la nature de la preuve ; le détail reste privé.

## États et clôture

États : `préparée`, `transmission déclarée`, `réponse reçue`, `réponse contrôlée`, `partielle`, `bloquée`, `clôturée`.

Une préparation de fichier n'est pas un envoi. Une réponse partielle ne clôt pas la demande entière. La conservation des sources et la récupération d'informations manquantes ont des critères de fin distincts ; suivre séparément ces deux résultats. Un échec de l'un n'empêche pas les travaux indépendants.

Pour la sauvegarde d'un lot privé : vérifier la bonne destination autorisée, les fichiers existants, l'absence de doublons/écrasement, le format d'origine et la relecture. Comparer taille et empreinte lorsque les outils l'autorisent. Un contrôle impossible est déclaré non effectué. Une archive simplement déposée n'est pas équivalente à la conservation individuelle demandée de ses pièces.

Si le titulaire transmet seulement un brief, commencer par rechercher les sources déjà présentes dans le Drive autorisé à partir des références privées qu'il fournit. Demander uniquement les pièces encore manquantes. Un inventaire, un brief PDF ou une extraction textuelle ne constitue pas la copie binaire d'un original absent.

Pour récupérer un historique : rendre le texte primaire effectivement retrouvé et sa provenance dans le canal privé ; séparer utilisateur et assistant, formulations originales et synthèses, séquence certaine et lacunes. Ne pas compléter les messages manquants par supposition.

## Relance et conflits

Reprendre le même identifiant si le besoin est identique. Avant une nouvelle écriture, relire l'état et la version pour éviter une relance en double ou l'écrasement d'une réponse plus récente. Un nouvel objectif distinct reçoit un nouvel identifiant.

Le contenu détaillé des preuves reste dans l'espace privé faisant autorité. GitHub conserve le mandat et le statut non sensibles ; il ne devient pas un second dossier RH. Les instantanés et copies ne sont pas des versions concurrentes faisant autorité.

## Automatisation future

Un déclencheur GitHub, une tâche Work, un accès Drive et une reprise Codex sont quatre capacités distinctes. Leur existence et leur chaîne complète doivent être vérifiées avant une automatisation. Ne pas activer de nouveau service, accès ou coût par la seule lecture de ce protocole. Le premier objectif est un relais manuel réussi de bout en bout.
