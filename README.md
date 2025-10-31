# ♟️ SQL Project: Online Chess Platform Database

## ✨ Summary  
This project designs and implements a **complete relational database system** for an online chess platform using **Oracle SQL** and **PL/SQL**.  
The work began with a **fully modeled relational diagram**, capturing every entity, key, and assumption of the platform before moving to SQL implementation.  

The database manages players, games, tournaments, clubs, teams, leagues, chats, and rewards — supporting realistic logic for tracking player performance, tournament activity, and reward management.  
Finally, the project integrates **automated triggers** and **analytical queries** to simulate platform dynamics and generate leaderboard insights.

---

## 🧩 Conceptual & Relational Design  
- Designed a **complete relational model** using *draw.io*, with more than 20 entities and clear key relationships.  
- Defined **domain constraints** (e.g., tournament type, gift category, result values).  
- Modeled **business assumptions**, such as:  
  - Tournament results cannot be recorded before the match date.  
  - Player ratings start at 1500 and change dynamically through triggers.  
  - Gifts can only be purchased if sufficient points and stock exist.  

This stage ensured data consistency and logical integrity before writing a single SQL statement.

---

## 🏆 Core Achievements & Contributions  

**Relational Schema Implementation**  
- Created normalized database structure for **PLAYERS**, **TOURNAMENTS**, **GAMES**, **CLUBS**, **TEAMS**, **GIFTS**, and **LEAGUES**.  
- Enforced referential integrity through **primary keys**, **foreign keys**, and **check constraints**.  

**Inheritance & Data Abstraction**  
- Implemented entity inheritance for `GIFT`, with two child tables: `MERCHANDISING` and `ONLINE_FEATURE`.  

**Business Logic Automation (Triggers)**  
- `BUY_GIFT`: Validates player rating and stock before purchase; updates both after confirmation.  
- `UPDATE_PLAYER_RATINGS`: Adjusts player scores automatically after each game.  
- `CHECK_PLAYERS_IN_CLUB`: Verifies player membership before inserting new game data.  
- `CODE_ASSIGNER`: Uses sequences to auto-assign club identifiers.  

**Data & Testing**  
- Inserted **150+ sample records** simulating active players, matches, and tournaments.  
- Validated logic through integrity checks and trigger testing.  

**Analytical Queries**  
- Generated player performance reports and club rankings.  
- Computed tournament participation metrics and white/black win ratios.  
- Analyzed gift purchasing trends over time.  

---

## 🧠 Technical Stack  

- **Database:** Oracle SQL  
- **Languages:** SQL (DDL, DML), PL/SQL  
- **Tools:** Draw.io (Relational Model), SQL Developer  
- **Techniques:** Database Modeling, Referential Integrity, Stored Logic, Analytical Query Design  

---

## ⚙️ Repository Contents  

| File | Description |
|------|--------------|
| `RelationalModel.drawio.pdf` | Conceptual and relational database diagram |
| `CREATION OF TABLES.sql` | Defines database schema (DDL) |
| `FOREIGN KEYS.sql` | Establishes foreign key relationships |
| `INSERTION OF RECORDS.sql` | Populates database with sample data |
| `QUERIES AND TRIGGERS.sql` | Contains triggers, sequences, and analytical queries |
| `DELETION OF TABLES.sql` | Optional cleanup script |

---

## 📈 Outcomes  

- Built a **robust and coherent SQL database** capable of tracking over **1,000 games** and player statistics.  
- Delivered **functional automation** for rating updates, reward purchases, and data validation.  
- Designed a **clear, normalized schema** ready for real application integration or data analysis extension.  

---

## 👥 Authors  

- Iván López Anca  
- Jiawei Xu
