# Centre Culturel Musulman de Longueuil DB

**قاعدة بيانات المسجد** — Base de données de la mosquée

Application de gestion des documents du centre : contrats de mariage (nikah),
certificats, attestations, reçus, registres, infolettres, calendrier islamique
et horaire des prières. Tout fonctionne dans un seul fichier, `index.html`,
sans serveur et sans connexion Internet.

> ⚠️ **Ce dépôt doit rester privé** (*Settings → General → Danger Zone → Change visibility → Private*).
> Il ne contient que le programme. **Ne jamais y ajouter de sauvegarde, d'export ou de document rempli.**

---

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html` | L'application complète |
| `assets/CCML-logo.png` | Logo, fond transparent (pour fonds clairs) |
| `assets/CCML-logo-light.png` | Logo pour fonds foncés |
| `assets/CCML-logo.svg` | Logo vectoriel (toute taille) |
| `LICENSE` | Licence propriétaire — tous droits réservés |
| `.gitignore` | Bloque les sauvegardes et exports contenant des données personnelles |

## Fonctionnalités

- **Contrats de mariage** : formulaire bilingue, copie de la mosquée (avec pièces d'identité) et copie des époux, en Word ou à l'impression.
- **Registre** : recherche, modification, export Excel, sauvegarde et restauration.
- **Documents** (28 types) : Shahada, attestations, lettres d'accommodement, Hajj/Omra, divorce religieux, reçus officiels de dons (exigences de l'ARC), zakat, procès-verbaux, école, annonces, infolettre…
- **Calendrier hégirien** (Umm al-Qura) avec les fêtes et occasions islamiques, et **horaire des prières** calculé pour Longueuil.
- **Écran de connexion** par mot de passe, verrouillage automatique après 30 minutes.

## Utilisation

1. Ouvrir `index.html` dans Chrome ou Edge, **toujours sur le même ordinateur et le même navigateur**.
2. Se connecter avec le mot de passe, puis le **changer** : *Documents → Paramètres du centre → Mot de passe*.
3. Remplir les *Paramètres du centre* (signataire, imam, numéro d'enregistrement d'organisme de bienfaisance).
4. Faire une **sauvegarde chaque mois** (*Registre → نسخة احتياطية*) et la conserver sur une clé USB chiffrée.

## Où sont les données ?

Les données **ne sont pas dans ce fichier ni dans ce dépôt**. Elles sont enregistrées
dans le navigateur de l'ordinateur où l'application est utilisée. Conséquences :

- Copier ou voler `index.html` ne donne accès à **aucun** dossier.
- Un autre navigateur ou un autre ordinateur affiche un registre vide.
- Effacer les données de navigation ou utiliser la navigation privée peut **effacer le registre**. Gardez des sauvegardes.
- Pour changer d'ordinateur : *sauvegarde* sur l'ancien, *restauration* sur le nouveau.

## Sécurité — à lire

- Le mot de passe est un **écran de confidentialité**, pas un chiffrement. Quiconque lit le code peut le contourner sur sa propre copie, et le mot de passe d'origine est trop simple pour résister. **Changez-le.**
- Les **fichiers de sauvegarde** contiennent tous les dossiers en clair (noms, numéros d'identité, adresses). Ne les envoyez jamais par courriel non protégé et **ne les ajoutez jamais à GitHub**.
- Protégez l'ordinateur lui-même : mot de passe de session Windows/Mac et chiffrement du disque (BitLocker / FileVault).
- Le `.gitignore` protège quand vous utilisez **Git ou GitHub Desktop**. **Le téléversement par glisser-déposer sur le site de GitHub ne l'applique pas** : n'y glissez que les fichiers de ce dossier.

## Mettre à jour l'application

1. Faire une sauvegarde depuis le *Registre*.
2. Remplacer l'ancien fichier par le nouveau, **au même endroit et sous le même nom**.
3. Si le registre paraît vide après la mise à jour, utiliser *Restauration* avec la sauvegarde.

## Avertissements

- Les heures de prière sont calculées (méthode ISNA par défaut) : comparez-les à l'horaire officiel de la mosquée et ajustez-les dans les paramètres.
- Les dates hégiriennes suivent le calendrier Umm al-Qura ; le début des mois peut différer d'un jour selon l'observation du croissant.
- Les attestations de divorce religieux n'ont aucun effet civil au Canada.
- N'émettez des reçus officiels aux fins de l'impôt que si le centre est un organisme de bienfaisance enregistré auprès de l'ARC.
- Les textes des lettres sont des modèles à faire valider par l'imam ; ils ne constituent pas un avis juridique.

---

## بالعربية — ملخص

تطبيق لإدارة وثائق المركز: عقود الزواج، والشهادات والإفادات، والإيصالات، والسجلات، والتقويم الهجري ومواقيت الصلاة، في ملف واحد `index.html` يعمل دون خادم ودون إنترنت.

- **اجعل هذا المستودع خاصاً (Private)**، ولا تضع فيه أبداً ملفات النسخ الاحتياطية أو الملفات المصدَّرة أو الوثائق المعبّأة.
- البيانات **ليست في هذا الملف**؛ إنها محفوظة في متصفح الجهاز الذي يُستعمل عليه التطبيق، فنسخ الملف لا يكشف أي سجل.
- غيّر كلمة المرور فور أول دخول، واحفظ نسخة احتياطية كل شهر في مكان آمن.
- كلمة المرور حاجب للخصوصية وليست تشفيراً؛ احمِ الجهاز نفسه بكلمة مرور وبتشفير القرص.
- ملف `.gitignore` يمنع رفع النسخ الاحتياطية عند استعمال Git أو GitHub Desktop، لكنه **لا يعمل عند السحب والإفلات في موقع GitHub**؛ فلا تسحب إلا ملفات هذا المجلد.

---

© 2026 Centre Culturel Musulman de Longueuil — Tous droits réservés. Voir [`LICENSE`](LICENSE).
