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

Testing : 
- Compile di Unity
- Klik Run untuk Test-run lewat Editor

Deploying : 
- Compile di Unity
- Build app sesuai target platform
- Run lewat hasil Build

## Classes Used

- BulletBehavior.cs
- DamageTrap.cs
- DungeonAudio.cs
- FadeAudioSource.cs
- FieldOfView.cs
- GameManager.cs
- GameSetting.cs
- JoystickScaler.cs
- LobbyAudio.cs
- MasterManager.cs
- OpenChest.cs
- PhotonConnect.cs
- PlaneCollider.cs
- PlayerManager.cs
- PlayerMovement.cs
- PlayerShoot.cs
- PlayerTagChanger.cs
- PlayerUi.cs
- PositionOfTraps.cs
- SingletonScriptableObject.cs
- SpawnThunders.cs
- SpellCastBound.cs
- StartMatch.cs
- ThunderManager.cs
- Timer.cs
- TransparentBush.cs

## Class Diagram
![alt text](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/654070f4-d406-4911-a8ba-d56e237203cb/Witchnesia-ClassDiagram-Battleground.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20201202%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20201202T041615Z&X-Amz-Expires=86400&X-Amz-Signature=0f9ff14c1d0117adfbbf5f7bac06ba23ac21ee21485f7112adddb04679f01c19&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Witchnesia-ClassDiagram-Battleground.png%22)


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
