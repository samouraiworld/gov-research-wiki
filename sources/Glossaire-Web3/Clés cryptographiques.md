
## 1. Définition

Les clés cryptographiques, base de l'authentification dans les protocoles de [[Blockchain]], repose sur le chiffrement asymétrique qui permet de réserver des informations aux seules personnes disposant des clefs adéquates, en garantissant une identification réciproque¹. 
Mise en oeuvre au sein des [[Wallet]], le processus permettant de générer un couple de clés cryptographiques utilise une courbe elliptique - l’algorithme ECDSA (Elliptic Curve Digital Signature Algorithm) pour Bitcoin. Cet algorithme dispose de procédures distinctes pour la signature et la vérification. La clé privée est utilisée pour signer les transactions. La clé publique, dérivée de la clé privée _via_ la courbe elliptique, est utilisée pour vérifier ces signatures. L’adresse Bitcoin est ensuite dérivée de la clé publique en appliquant les fonctions de hachage SHA-256 et RIPEMD-160, suivies du format d’encodage Base58Check pour faciliter l’utilisation et la vérification. Voir 

## 2. Rapprochement & Tensions

## 3. Exemples concrets

## 4. Risques & Opportunités

## 5. Sources & Références

 ¹ Hughes Eric, 1993, « A Cypherpunk’s Manifesto », https://www.activism.net/cypherpunk/manifesto.html, 9 mars 1993, consulté le 6 mai 2020.
2Rykwalder Eric, 2014, « The Math Behind Bitcoin », https://www.coindesk.com/math-behind-bitcoin, 19 octobre 2014, consulté le 4 août 2020.