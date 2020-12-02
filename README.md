# WITCHGAME : MAGICAL BATTLE ARENA

This repository is a final project from Object-Oriented Programming Class, Teknik Informatika Universitas Padjadjaran. 

[Challenge Guidelines](challenge-guideline.md)

WitchGame: Magical Battle Arena adalah Dungeon Multiplayer Twin-Stick Shooter di mana Para Pemain sebagai Penyihir, bersaing satu sama lain di dungeon sambil menghindari jebakan dan  perubahan lingkungan. Pemenangnya adalah orang yang mengumpulkan orb dari dungeon, dengan cara mengeliminasi pemain lain atau Membunuh monster Penjaga yang bersembunyi di dungeon. 

## Credits
| NPM           | Name              |
| ------------- |-------------------|
| 140810140054  | Ridha Septia      |
| 140810160005  | Dio Tri Satyaloka |


## Change log
- **[Sprint Planning](changelog/sprint-planning.md) - (17/11/2020)** 
   - Discussion about the planning of the project

- **[Sprint 1](changelog/sprint-1.md) -  (date from 17/11/2020 until 22/11/2020)** 
   - Photon Test Part 1
   - Player Movement 
   - Health and shooting
   - Spells development

- **[Sprint 2](changelog/sprint-2.md) - (date from 23/11/2020 until 30/11/2020)** 
   - Player Score
   - Fog of War
   - Photon Test Part 2
   - Guardian chase, patrol, attack
   
- **[Sprint 3](changelog/sprint-3.md) - (date from x until x)** 
   - Mini Boss
   - FSM - Spell System Prototype
   - The Weather Event
   - Implementation Networking

## Running The App

TO;DO with steps

## Classes Used

TO;DO

UML image here

## Notable Assumption and Design App Details

- Matchmaking Dilakukan secara Acak.
- Satu match terdiri dari 4 Player, dan 1 Non-Player Enemy.
- Setiap match memiliki timer yang terdiri dari 3 phase, fase collecting points, roaming/weather event, dan boss fight.
- Dalam satu map terdapat sekumpulan orbs yang bisa diambil player. Orb ini memberikan poin.
- Setiap Player mengendalikan sebuah karakter Witch, yang memiliki 2 spell/skill dan basic attack.
- Player bisa menggunakan Spell dan Attack untuk menyerang dan membunuh player lain.
- Jika karakter player mati, skor poin akan dikurangi. 
- Pemenang ditentukan dari pemilik poin terbanyak.
- Setelah timer phase mencapai 0:00, match selesai. Akan ditampilkan siapa pemenangnya, dan player bisa kembali ke menu utama.
