# matos-kali-full.md
# PC pour développement / pentest / bug-bounty — dual-boot Windows 11 / Kali Linux
**But** : machines (portables + desktops) neuves, TTC France, budget ciblé €800–1700.  
Priorités : CPU récent (Intel H-series 13/14ᵉ gen ou Ryzen 7/9 série 7000), **32–64 GB DDR5**, NVMe 512→1000 GB, design pro, Wi-Fi remplaçable ou Intel.

---

## Sommaire
1. Top 6 portables orientés hacking / dev (neuf, France)
2. Top 4 desktops (puissance / évolutivité)
3. Tableau récapitulatif
4. Exemple complet **PC à monter** (pièces + prix indicatifs + pourquoi)
5. Accessoires recommandés (dongles, backup, boîtes)
6. Checklist d’achat & d’installation (Win11 + Kali)
7. Notes pratiques & sources

---

## 1) Top 6 portables (orientés dev / pentest / dual-boot Kali)
> Choisis selon priorité : **mobilité** (poids/autonomie) vs **puissance** (CPU cores / nombre de slots / refroidissement). Vérifie avant achat : nombre de slots M.2, si RAM est soudée, et chipset Wi-Fi (préférer Intel).

### 1. Framework Laptop (13 / 16) — **modulaire / réparable**
- **Pourquoi** : remplaçable Wi-Fi/M.2/RAM, excellente réparabilité — parfait pour garantir compatibilité Kali (remplacement carte Wi-Fi si besoin).
- **Config cible** : Intel 13/14ᵉ gen / Ryzen récent, **32 GB DDR5**, NVMe 1 To.
- **Prix indicatif** : ~€900–€1 400 (selon CPU/RAM).

### 2. TUXEDO Pulse 15 (Gen2) — **Linux-first**
- **Pourquoi** : préconfigurable pour Linux, très bonne upgradabilité (2×M.2), livraison EU.
- **Config cible** : Ryzen 7/9 mobile, **32–64 GB DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 100–€1 800.

### 3. Slimbook Evo 15 — **Linux-first & value**
- **Pourquoi** : vendu pour Linux, bonnes options RAM, dual NVMe possible.
- **Config cible** : Ryzen AI / Ryzen 7/9, **32–64 GB DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 000–€1 600.

### 4. Dell XPS 15 — **Developer Edition (Ubuntu)**
- **Pourquoi** : bon support Ubuntu / hardware; solide par défaut pour Linux.
- **Config cible** : i7/i9 H-series, **32 GB DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 200–€1 700.

### 5. Lenovo ThinkPad T14/T16 / X1 Carbon (Intel) — **business**
- **Pourquoi** : historique Linux-friendly, BIOS flexible, clavier excellent pour dev.
- **Config cible** : i7 H/Ultra, **32 GB DDR5**, 512→1 To NVMe (vérifier slots).
- **Prix indicatif** : ~€1 000–€1 700.

### 6. Gigabyte AERO / Creator / ASUS Pro (Zephyrus creator variants)
- **Pourquoi** : format “creator” (pas gamer), bonnes dalles, slots M.2, refroidissement solide.
- **Config cible** : Ryzen 9 / i7 H, **32–64 GB DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 200–€1 800.

---

## 2) Top 4 desktops (meilleure perf /€ / évolutivité)  
> Si tu peux sacriﬁer la mobilité, desktop = meilleur rapport perf / prix et plus simple à préparer pour forensics (2 disques physiques).

### A — Desktop « équilibré / workstation »
- **CPU** : AMD **Ryzen 9 7900X** (12c/24t) ou Ryzen 7 7800X3D (selon dispo/prix)
- **RAM** : 32–64 GB DDR5
- **GPU** : RTX 4060 Ti (ou 4070 si budget)
- **Stockage** : NVMe 1 To + NVMe/SSD secondaire
- **Prix approximatif** : €1 200–€1 700 (monté / pièces)

### B — Desktop « CPU-first » (compilation / VM intensive)
- **CPU** : Intel i7-13700K / i7-14700 (ou Ryzen 9 selon promo)
- **RAM** : 64 GB DDR5
- **GPU** : GPU milieu (RTX 4060) pour CAO légère
- **Prix** : €1 300–€1 800

### C — Desktop « forensics » (max stockage / duplications)
- **CPU** : Ryzen 7/9
- **RAM** : 32–64 GB
- **Stockage** : 2×NVMe (isolation OS), 1×HDD 4 To pour images
- **Network** : carte PCIe Ethernet 2.5/10Gb optional

### D — System76 Thelio (desktop Linux-native)
- **Pourquoi** : vendu pour Linux, BIOS & support adaptés, facile à monter/configurer pour Tsurugi/Kali.

---

## 3) Tableau comparatif synthétique

| Modèle (catégorie) | CPU typique | RAM cible | SSD | Slots M.2 | Wi-Fi | Prix indicatif (TTC FR) | Points forts |
|---|---:|---:|---:|---:|---:|---:|---|
| Framework Laptop 13/16 | Intel 13/14 / Ryzen | 32–64 GB | 512–1 TB NVMe | facile | M.2 remplaçable | €900–1 400 | modularité, remplacement Wi-Fi |
| TUXEDO Pulse 15 Gen2 | Ryzen7/9 | 32–64 GB | 1 TB NVMe | 2×M.2 | Intel option | €1 100–1 800 | Linux-first, shop EU |
| Slimbook Evo 15 | Ryzen AI / 7/9 | 32–64 GB | 1 TB NVMe | 2×M.2 | Intel possible | €1 000–1 600 | Linux vendor, bon prix |
| Dell XPS 15 (Dev) | i7/i9 H | 32 GB (64 possible) | 512–1 TB NVMe | 2×M.2 (selon SKU) | Intel/Dev | €1 200–1 700 | design pro, support Ubuntu |
| ThinkPad T14/T16 / X1 | i7 H/Ultra | 32–64 GB | 512–1 TB NVMe | 1–2×M.2 | remplaçable | €1 000–1 700 | robust, clavier, BIOS ok |
| Gigabyte AERO / ASUS Pro | Ryzen/i7 H | 32–64 GB | 1 TB NVMe | 2×M.2 | vérif. chipset | €1 200–1 800 | écran colorimétrique, perf |
| Desktop Ryzen 7/9 custom | Ryzen 7/9 | 32–64 GB | 1 TB NVMe + 2ᵉ | 2+ | PCIe Wi-Fi | €900–1 700 | perf/€, évolutivité |

---

## 4) Exemple COMPLET : **PC à monter (desktop)** — configuration optimale pour dev / pentest / dual-boot
> Objectif : "meilleure config pour développement / pentest / VM / CAO légère" tout en restant dans un budget raisonnable (~€1 300–1 600 selon prix marché). J'indique **pièce**, **référence suggérée**, **pourquoi**, et **prix approximatif TTC (€)**.

> **Note** : prix indicatifs — vérifie promos. J’ai choisi composants Linux-friendly (Intel/AMD + Intel Wi-Fi option possible).

### A) Composants (suggestion)
1. **Processeur (CPU)**  
   - AMD **Ryzen 9 7900X** — 12c/24t, excellent multi-thread pour compilations/VM.  
   - **Prix indicatif** : **€320**

2. **Carte mère (MB)**  
   - *B650 / B650E ATX* (ex. Gigabyte B650 Aorus Elite AX / MSI MAG B650 Tomahawk) — 2×M.2, bonnes phases d’alimentation.  
   - **Prix indicatif** : **€150–€190**

3. **Mémoire (RAM)**  
   - **32 GB (2×16) DDR5-6000 CL32** (Crucial / Corsair / Kingston) — kit XMP, faible latence.  
   - Si budget le permet : **64 GB (2×32)** pour heavy VM.  
   - **Prix indicatif** : 32GB ≈ **€130–€160** ; 64GB ≈ **€260–€320**

4. **Stockage NVMe principal**  
   - **1 TB NVMe PCIe 4.0** (ex. Samsung 990 PRO ou équivalent) — RAPIDE pour OS & VMs.  
   - **Prix indicatif** : **€120–€150**

5. **Carte graphique (GPU)**  
   - **NVIDIA RTX 4060 Ti** (ou RTX 4060 si budget serré) — bon ratio perf/consommation ; utile pour accélération CAO & CUDA.  
   - **Prix indicatif** : RTX 4060 ≈ **€350–€400** ; 4060 Ti ≈ **€420–€520**

6. **Alimentation (PSU)**  
   - **Seasonic / Corsair / Be Quiet! 650–750W 80+ Gold (semi-modulaire)** — headroom pour upgrades.  
   - **Prix indicatif** : **€80–€110**

7. **Boîtier**  
   - ATX mid-tower avec bon airflow (ex. Fractal, NZXT, Phanteks) + 2–3 front fans.  
   - **Prix indicatif** : **€60–€100**

8. **Refroidissement CPU**  
   - Air cooler performant (Noctua NH-U12S redux / be quiet Dark Rock 4) ou AIO 240mm si tu veux silence.  
   - **Prix indicatif** : **€50–€110**

9. **Carte Wi-Fi (optionnelle)**  
   - **Intel AX210 / AX211 M.2** (pour Linux compatibility & monitor mode with supported drivers) — très conseillé pour Kali/Tsurugi.  
   - Ou prévoir **dongle USB Alfa AWUS** (pour injection/monitor).  
   - **Prix indicatif** : AX210 ≈ **€25–€40** ; Alfa AWUS ≈ **€30–€70**

10. **Extras**  
    - Câbles, pasta thermique, adaptateurs M.2 screw kit, ventilateurs supplémentaires.  
    - **Prix indicatif** : **€20–€40**

### B) Estimation totale (approx.)
- CPU €320  
- MB €170  
- RAM 32GB €140  
- NVMe 1TB €130  
- GPU 4060Ti €450  
- PSU €95  
- Boîtier €80  
- Cooler €60  
- Wi-Fi AX210 €35  
**→ Total ≈ €1 480** (≈ €1 350–1 650 selon modèle GPU / promos / choix 32 vs 64 GB)

> Si tu veux 64 GB → ajoute ~€160 → total ≈ €1 640.  
> Si tu choisis RTX 4070, le GPU fera grimper le total de ~€200–€350 (selon stock), poussant au-delà de €1 800.

### C) Pourquoi cette configuration ?  
- **Ryzen 9 7900X** : excellente puissance multi-thread pour builds et VMs.  
- **32→64 GB DDR5** : mémoire cruciale pour exécuter plusieurs VMs (Kali, sandboxes, etc.).  
- **NVMe 1 To** : rapidité pour OS/VM/IO.  
- **RTX 4060Ti** : GPU utile pour CAO légère, tests CUDA, accélérations — mais ce n’est pas indispensable pour pentest.  
- **Intel AX210 Wi-Fi** : meilleur support Linux, stable pour monitor/injection (ou utiliser dongle USB dédié).

---

## 5) Accessoires recommandés
- **Dongle Wi-Fi USB pour injection/monitor** : Alfa AWUS036NHA (Atheros) ou équivalent (très utile si la carte interne n’est pas compatible).  
- **Enclosure NVMe → USB 3.2 Gen2** (pour backups/clonage)  
- **Station dock / USB-C hub** (RJ45 gigabit, USB A, HDMI)  
- **SSD 2,5" ou HDD 4 To** pour stockage d’images forensiques  
- **On-the-go LiveUSB kit** : 2× LiveUSB (Kali + rescue), un lecteur USB fiable (brand Sandisk / Kingston 32→64GB)

---

## 6) Checklist d’achat & d’installation (Win11 + Kali)
### Avant d’acheter
- [ ] Vérifier nombre de **M.2 + baie 2.5"**  
- [ ] Vérifier si **RAM est soudée** (éviter si tu veux 64GB)  
- [ ] Vérifier **Wi-Fi chipset** (privilégier Intel AXxxx) ou la possibilité de le remplacer  
- [ ] Vérifier possibilité de **désactiver Secure Boot** dans le BIOS/UEFI  
- [ ] Lecture des retours de la communauté (reddit / forums / Github issues) pour modèle exact

### Pré-installation
1. **Créer images** : clone disque Windows actuel (si migration).  
2. **Créer LiveUSBs** : Kali Live + Rescue/Win installer.  
3. **Désactiver Secure Boot** (ou savoir signer bootloader).  
4. **Installer Tsurugi/Kali** sur NVMe#1 (ou partition dédiée). Test hardware en Live.  
5. **Installer Windows** sur NVMe#2 (si dual-disk) ou partition séparée.  
6. **Configurer GRUB / boot order** pour choisir l’OS ; garder LiveUSB de secours.  
7. **Installer drivers** : Intel Wi-Fi drivers, audio, GPU drivers (NVIDIA proprietary si besoin sous Windows).

---

## 7) Notes pratiques & recommandations finales
- **Si tu veux “just works” sous Linux** et réduire le temps de bidouille → achète chez un vendor Linux-first (System76 / Tuxedo / Slimbook / Framework).  
- **Si tu veux la meilleure perf par €** → desktop custom (Ryzen 7/9) est généralement meilleur rapport perf/prix qu’un portable équivalent.  
- **Dongle Wi-Fi** (USB) est un investissement faible mais souvent indispensable pour pentesting (monitor/injection).  
- **Sécurité / forensic** : isole les OS sur disques physiques quand possible ; chiffre les partitions sensibles (LUKS) pour protéger les données.

---

### Ressources utiles (doc & guides)
- Kali docs — Dual boot with Windows: https://www.kali.org/docs/installation/dual-boot-kali-with-windows/  
- Tsurugi Linux — downloads & docs: https://tsurugi-linux.org/  
- Framework marketplace: https://frame.work/marketplace/laptops  
- Tuxedo Computers: https://www.tuxedocomputers.com  
- System76: https://system76.com

---
