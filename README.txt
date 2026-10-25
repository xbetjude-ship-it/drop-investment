DROP INVESTMENT — prototype de site statique

CONTENU
- index.html : page responsive en français, interface de compte membre de démonstration et calculateur hypothétique.
- affiche-reference.png : visuel de référence, si disponible.

IMPORTANT
Cette version est un prototype front-end uniquement :
- aucune authentification réelle ; ne saisit aucun vrai mot de passe ;
- aucun compte client n'est créé sur un serveur ;
- aucun paiement, dépôt ou retrait réel ;
- aucun rendement garanti.
Pour passer en production, il faut développer une API/backend sécurisé, une base de données, une authentification fiable, la validation serveur de toutes les opérations, une journalisation et une intégration avec un prestataire de paiement autorisé. Vérifier au préalable les exigences légales et réglementaires applicables.

HÉBERGEMENT SUR NETLIFY (site statique)
1. Téléchargez et décompressez drop_investment_site.zip.
2. Ouvrez https://app.netlify.com/ et connectez-vous ou créez un compte.
3. Dans le tableau de bord, choisissez Add new site / Deploy manually (le libellé peut varier).
4. Glissez-déposez le dossier décompressé qui contient directement index.html (et affiche-reference.png).
5. Attendez la fin du déploiement. Netlify affichera une adresse en *.netlify.app.
6. Ouvrez cette adresse sur téléphone pour tester les liens et le formulaire de démonstration.
7. Pour modifier le site, changez index.html puis redéployez le dossier mis à jour.
8. Pour un nom de domaine personnalisé, allez dans Domain management et suivez les instructions Netlify.

Netlify héberge ici les fichiers statiques. Il ne fournit pas à lui seul une authentification de production ni une gestion financière sécurisée.


PAIEMENT CRYPTO — ÉTAPE SUIVANTE
La maquette propose des choix de crypto (USDT TRC20, BTC, ETH, USDT ERC20), mais ne reçoit pas d'argent.
Avant d'activer de vrais paiements :
- choisissez précisément la cryptomonnaie et le réseau ;
- créez ou choisissez un portefeuille professionnel dont vous contrôlez les clés ;
- ne publiez jamais de phrase de récupération ou de clé privée ;
- utilisez une intégration serveur ou un prestataire de paiement crypto fiable pour générer des adresses/ordres, suivre les confirmations et empêcher les validations falsifiées ;
- prévoyez les remboursements, les frais, le support et les vérifications légales applicables.
Ne collez pas une adresse inventée : l'adresse et le réseau doivent être vérifiés par le propriétaire du portefeuille.


CONFIGURATION DU PAIEMENT BITCOIN (BTC) — PAS ENCORE ACTIVÉ
Le site affiche maintenant Bitcoin uniquement pour le mode de réception par portefeuille.
Aucune adresse BTC n'a été inventée ou intégrée. Aucun paiement n'est actif.

Avant de passer en production :
1. Créez ou choisissez un portefeuille Bitcoin que vous contrôlez. Sauvegardez sa phrase de récupération hors ligne et ne la partagez jamais.
2. Seule l'adresse publique de réception BTC pourra être utilisée sur le site. Ne saisissez ni phrase de récupération, ni clé privée, ni code PIN dans le site ou dans un chat.
3. Faites vérifier l'adresse publique et le réseau Bitcoin par une personne de confiance, idéalement avec un petit test.
4. Pour un vrai site avec comptes clients, ne validez jamais un dépôt sur la seule base d'une capture d'écran. Le serveur doit vérifier la transaction on-chain, le montant, l'adresse destinataire, le nombre de confirmations et empêcher qu'une même transaction soit créditée deux fois.
5. Gardez les clés privées hors du serveur web. Pour générer des adresses de dépôt par client, utilisez une architecture wallet dédiée et auditée ou un prestataire qualifié.
6. Ajoutez une procédure claire pour les erreurs de réseau, remboursements, frais, support et réclamations.
7. Vérifiez les obligations légales et réglementaires applicables avant de collecter des fonds ou de proposer un produit d'investissement.

La maquette Netlify est un site statique : elle ne peut pas, seule, vérifier la blockchain ni gérer des soldes clients de façon sécurisée. Un backend et une base de données sécurisés sont indispensables.
