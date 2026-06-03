# 🌍 Le Lovethon — Dictionnaire Mondial de l'Amour

Ce projet intègre un dictionnaire multilingue qui permet à l'appareil photo de reconnaître les expressions d'affection et les mots doux à travers le monde pour déclencher la capture.

---

## 🗂️ Liste des mots clés supportés

Voici les termes exacts configurés dans le script pour déclencher instantanément la photo :

| Langue / Origine | Mots clés reconnus |
| :--- | :--- |
| **Français** | `je t'aime`, `amour`, `mon cœur`, `mon coeur`, `chéri`, `chérie`, `je taime`, `adore`, `aimer`, `mon ange` |
| **Anglais** | `i love you`, `love`, `my love`, `sweetheart`, `darling`, `babe`, `forever`, `honey` |
| **Espagnol** | `te amo`, `te quiero`, `amor`, `mi amor`, `corazón`, `corazon`, `cariño`, `carino` |
| **Italien** | `ti amo`, `amore`, `amore mio`, `tesoro`, `ti voglio bene` |
| **Allemand** | `ich liebe dich`, `liebe`, `mein schatz`, `schatz` |
| **Portugais** | `eu te amo`, `amor`, `meu amor`, `querido`, `querida` |
| **Arabe** | `habibi`, `habibti`, `bahebak`, `ana bahebak`, `ya rouhi` |
| **Turc** | `seni seviyorum`, `aşkım`, `askim`, `sevgilim` |
| **Néerlandais** | `ik hou van jou`, `liefde` |
| **Russe** | `ya tebya lyublyu`, `lyubov`, `lyublyu` |
| **Japonais** | `aishiteru`, `daisuki`, `anata` |
| **Coréen** | `saranghae`, `saranghaeyo` |
| **Chinois** | `wo ai ni` |

---

## 💻 Intégration JavaScript

Le tableau est traité en minuscules pour assurer une détection fluide et insensible à la casse lors de l'écoute active :

```javascript
const loveWords = [
    "je t'aime", "amour", "mon cœur", "mon coeur", "chéri", "chérie", "je taime", "adore", "aimer", "mon ange",
    "i love you", "love", "my love", "sweetheart", "darling", "babe", "forever", "honey",
    "te amo", "te quiero", "amor", "mi amor", "corazón", "corazon", "cariño", "carino",
    "ti amo", "amore", "amore mio", "tesoro", "ti voglio bene",
    "ich liebe dich", "liebe", "mein schatz", "schatz",
    "eu te amo", "amor", "meu amor", "querido", "querida",
    "habibi", "habibti", "bahebak", "ana bahebak", "ya rouhi",
    "seni seviyorum", "aşkım", "askim", "sevgilim",
    "ik hou van jou", "liefde", "ya tebya lyublyu", "lyubov", "lyublyu",
    "aishiteru", "daisuki", "anata", "saranghae", "saranghaeyo", "wo ai ni","ti amo"
];
