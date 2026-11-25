# IGT PRESENCE

Interface web de gestion des présences — Inspection Générale du Travail, RDC.

## Publication
Le workflow GitHub Actions `.github/workflows/pages.yml` publie automatiquement le contenu de la branche `main` sur GitHub Pages à chaque mise à jour.

Dans GitHub : **Settings → Pages → Build and deployment → Source : GitHub Actions**.

## État fonctionnel actuel
- Interface responsive et tableau de bord de démonstration.
- Directions du périmètre pilote Administration Centrale / Kinshasa-Gombe.
- Formulaire d'ajout manuel en mode démonstration local.
- Recherche et export CSV des demandes locales.

## À raccorder avant une utilisation réelle
La connexion Supabase et les opérations sécurisées ne sont pas activées dans cette version. Les demandes du formulaire restent dans la mémoire de la page et ne sont pas enregistrées dans la base. Le registre officiel, les pointages, les validations serveur, les comptes et les terminaux ne sont donc pas opérationnels ici.

Ne jamais placer une clé Supabase `service_role` dans le navigateur. Les écritures doivent passer par des Edge Functions avec authentification, contrôle des rôles et journalisation. La reconnaissance faciale et la biométrie ne sont pas activées.

## Déploiement
Après avoir activé GitHub Pages avec GitHub Actions, le site sera disponible à :
https://limengosocrate.github.io/Igt-pr-sence-/
