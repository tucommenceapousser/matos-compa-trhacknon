# matos-kali-full.md
## PC pour développement / pentest / bug-bounty — dual-boot Windows 11 / Kali Linux
**But** : machines (portables + desktops) neuves, TTC France, budget ciblé €800–1700.  
Priorités : CPU récent (Intel H-series 13/14ᵉ gen ou Ryzen 7/9 série 7000), **32–64 Go DDR5**, NVMe 512→1000 Go, design pro, Wi-Fi remplaçable ou Intel.

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
- **Config cible** : Intel 13/14ᵉ gen / Ryzen récent, **32 Go DDR5**, NVMe 1 To.
- **Prix indicatif** : ~€900–€1 400 (selon CPU/RAM).
- ![Framework Laptop](https://www.framework.com/assets/images/hero.jpg)

### 2. TUXEDO Pulse 15 (Gen2) — **Linux-first**
- **Pourquoi** : préconfigurable pour Linux, très bonne upgradabilité (2×M.2), livraison EU.
- **Config cible** : Ryzen 7/9 mobile, **32–64 Go DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 100–€1 800.
- ![TUXEDO Pulse 15](https://www.tuxedocomputers.com/media/image/thumbnail/800x600/7e/2b/3e/TUXEDO_Pulse_15_Gen2_2023_1.jpg)

### 3. Slimbook Evo 15 — **Linux-first & value**
- **Pourquoi** : vendu pour Linux, bonnes options RAM, dual NVMe possible.
- **Config cible** : Ryzen AI / Ryzen 7/9, **32–64 Go DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 000–€1 600.
- ![Slimbook Evo 15](https://slimbook.com/wp-content/uploads/2023/06/slimbook-evo-15-2023.jpg)

### 4. Dell XPS 15 — **Developer Edition (Ubuntu)**
- **Pourquoi** : bon support Ubuntu / hardware; solide par défaut pour Linux.
- **Config cible** : i7/i9 H-series, **32 Go DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 200–€1 700.
- ![Dell XPS 15](https://i.dell.com/sites/csimages/Merchandizing_Imagery/all/xps-15-9520-laptop.jpg)

### 5. Lenovo ThinkPad T14/T16 / X1 Carbon (Intel) — **business**
- **Pourquoi** : historique Linux-friendly, BIOS flexible, clavier excellent pour dev.
- **Config cible** : i7 H/Ultra, **32 Go DDR5**, 512→1 To NVMe (vérifier slots).
- **Prix indicatif** : ~€1 000–€1 700.
- ![Lenovo ThinkPad T14](https://www.lenovo.com/medias/lenovo-laptop-thinkpad-t14-gen-1-hero.png)

### 6. Gigabyte AERO / Creator / ASUS Pro (Zephyrus creator variants)
- **Pourquoi** : format “creator” (pas gamer), bonnes dalles, slots M.2, refroidissement solide.
- **Config cible** : Ryzen 9 / i7 H, **32–64 Go DDR5**, 1 To NVMe.
- **Prix indicatif** : ~€1 200–€1 800.
- ![Gigabyte AERO Creator](https://www.gigabyte.com/FileUpload/Global/KeyFeature/2021/2021_AERO_17_HDR/2021_AERO_17_HDR_01.jpg)

---

## 2) Top 4 desktops (meilleure perf /€ / évolutivité)
> Si tu peux sacrifier la mobilité, desktop = meilleur rapport perf / prix et plus simple à préparer pour forensics (2 disques physiques).

### A — Desktop « équilibré / workstation »
- **CPU** : AMD **Ryzen 9 7900X** (12c/24t) ou Ryzen 7 7800X3D (selon dispo/prix)
- **RAM** : 32–64 Go DDR5
- **GPU** : RTX 4060 Ti (ou 4070 si budget)
- **Stockage** : NVMe 1 To + NVMe/SSD secondaire
- **Prix approximatif** : €1 200–€1 700 (monté / pièces)
- ![AVADirect Ryzen 9 7900X + RTX 4060 Ti](https://www.avadirect.com/Images/Products/18747962/18747962_1.jpg)

### B — Desktop « CPU-first » (compilation / VM intensive)
- **CPU** : Intel i7-13700K / i7-14700 (ou Ryzen 9 selon promo)
- **RAM** : 64 Go DDR5
- **GPU** : GPU milieu (RTX 4060) pour CAO légère
- **Prix** : €1 300–€1 800
- ![iBUYPOWER Ryzen 9 9900X + Radeon RX 9070 XT](https://www.ibuypower.com/Images/Products/Store/PCs/UltimateGamingPC/UltimateGamingPC_1.jpg)

### C — Desktop « forensics » (max stockage / duplications)
- **CPU** : Ryzen 7/9
- **RAM** : 32–64 Go
- **Stockage** : 2×NVMe (isolation OS), 1×HDD 4 To pour images
- **Network** : carte PCIe Ethernet 2.5/10Gb optional
- ![Velztorm White Armix](https://www.newegg.com/3D5-000W-19VU0/image/3D5-000W-19VU0-1.jpg)

### D — System76 Thelio (desktop Linux-native)
- **Pourquoi** : vendu pour Linux, BIOS & support adaptés, facile à monter/configurer pour Tsurugi/Kali.
- ![System76 Thelio](https://system76.com/sites/default/files/styles/product_page/public/2021-04/Thelio_Desktop_1.jpg)

---

## 3) Tableau comparatif synthétique

| Modèle (catégorie) | CPU typique | RAM cible | SSD | Slots M.2 | Wi-Fi | Prix indicatif (TTC FR) | Points forts |
|--------------------|-------------|-----------|-----|-----------|-------|-------------------------|--------------|
| Framework Laptop 13/16 | Intel 13/14 / Ryzen | 32–64 Go | 512–1 To NVMe | facile | M.2 remplaçable | €900–1 400 | modularité, remplacement Wi-Fi |
| TUXEDO Pulse 15 Gen2 | Ryzen7/9 | 32–64 Go | 1 To NVMe | 2×M.2 | Intel option | €1 100–1 800 | Linux-first, shop EU |
| Slimbook Evo 15 | Ryzen AI / 7/9 | 32–64 Go | 1 To NVMe | 2×M.2 | Intel possible | €1 000–1 600 | Linux vendor, bon prix |
| Dell XPS 15 (Dev) | i7/i9 H | 32 Go (64 possible) | 512–1 To NVMe | 2×M.2 (selon SKU) | Intel/Dev | €1 200–1 700 | design pro, support Ubuntu |
| ThinkPad T14/T16 / X1 | i7 H/Ultra | 32–64 Go | 512–1 To NVMe | 1–2×M.2 | remplaçable | €1 000–1 700 | robust, clavier, BIOS ok |
| Gigabyte AERO / ASUS Pro | Ryzen/i7 H | 32–64 Go | 1 To NVMe | 2×M.2 | vérif. chipset | €1 200–1 800 | écran colorimétrique, perf |
| Desktop Ryzen 7/9 custom | Ryzen 7/9 | 32–64 Go | 1 To NVMe + 2ᵉ | 2+ | PCIe Wi-Fi | €900–1 700 | perf/€, évolutivité |

---

## 4) Exemple COMPLET : **PC à monter (desktop)** — configuration optimale pour dev / pentest / dual-boot
> Objectif : "meilleure config pour développement / pentest / VM / CAO légère" tout en restant dans un budget raisonnable (~€1 300–1 600 selon prix marché). J'indique **pièce**, **référence suggérée**, **pourquoi**, et **prix approximatif TTC (€)**.

> **Note** : prix indicatifs — vérifie promos. J’ai choisi composants Linux-friendly (Intel/AMD + Intel Wi-Fi1
