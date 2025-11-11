# 🍎 Save The Fruits - Internal Live Data System

## ⚠️ Internal Use Only (Bubencillos Team)

This repository is the **exclusive, internal control center** for managing and deploying game data for **Save The Fruits**.

We use this system to send updated prices, weapons statistics, and level configurations directly to our live servers without requiring any restarts (Zero-Downtime Patching).

**DO NOT** make this repository public. **All contents are proprietary to the Bubencillos Team.**

## ✨ Data Managed by This System

This system handles everything formatted in **JSON**. It is used solely for rapid data changes and game balancing.

| Content Type | Purpose | Example of a Change |
| :--- | :--- | :--- |
| **Statistics** | Item prices, ability damage, enemy health points. | Increasing the damage of the "Mango Bomb" from 10 to 15. |
| **Configuration** | Level rules, fruit spawn rates, game difficulty settings. | Adjusting the difficulty curve for the "Pineapple Phase". |
| **Texts** | Internal text strings, logs, and development messages. | Correcting a developer-facing error message. |

## ⚙️ Deployment Workflow (Bubencillos Process)

This process allows for instant data updates on the live server:

1.  **Change:** A team member edits a `.json` file in their local branch.
2.  **Review:** The change is reviewed by the lead developer and merged into the `main` branch.
3.  **Deployment:** Our CI/CD pipeline or internal script automatically pushes the updated `.json` file to the server's data directory.
4.  **Live Reload:** The Game Server Core detects the file change and instantly loads the new data into memory.

**Result:** The updated data is live in-game **within seconds** for all active players.

## 📂 Key Data Structure

The most important data files are structured as follows:

| File/Folder | Content |
| :--- | :--- |
| `data/stats.json` | Numerical stats for all fruits, enemies, and abilities. |
| `data/levels/` | JSON files defining each game level or stage. |
| `config.json` | Core server and general game configuration settings. |

---

## 🚫 Licensing and Ownership

All data and content within this repository are the **exclusive and proprietary property of Bubencillos.** This is **not** an Open Source project.

## 📞 Contact

Developed and maintained exclusively by the **Bubencillos** Team.

* **GitHub Owner:** [@Bubencillos](https://github.com/Bubencillos)
* **Discord:** [@devbuben](https://discord.com/users/987175599699292220)
* **Mail:** [bubencillos@gmail.com](mailto:bubencillos@gmail.com)



