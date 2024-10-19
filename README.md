# Friendly GTFO

## Description

Multiple tweaks to scale down difficulty for non-hardcore gamers.

Most likely will not work with other Rundown Mods that edit the same DataBlocks.

### Balance Changes:

Mostly testing with `GregSlythe-Solo_Mode` enabled.

#### Weapons:

- Doubled damage

#### Flashlights:

- Wider angle for all flashlights.

#### Player stats:

- `2 times` effective health.
- Faster regen speed and delay: `5%/second`, `3 seconds after damage`.
- Regen limit: `20% -> 100%`
- `17%` faster movement speed.
- Stamina no longer affects :
	- `Movement speed`
	- `Melee speed`
	- `Breathing`

#### Melee:

- All charge attack damage is doubled.

## Changelog

### 3.0.0

- Remade for Rundown 8.0

### 2.1.1

Fixed README Description.

> god will i ever actually release a README without any typos.

### 2.1.0

> nerfs! game was way too easy now!

#### Player:

- Nerfed Health in general.
	- `"health": 100.0 -> 50.0`
	- `"healthRegenStartDelayAfterDamage": 3.0 -> 5.0`
	- `"healthRegenRelMax": 0.5 -> 0.6`
	- `"healthRegenPerSecond": 3.0 -> 2.5`

	> after increasing movement speed for faster exploration,
	> it made evading attacks much easier, which made a fun experience.
	> im going to double down on this and instead make overall health lower than before.

- Nerfed Ammo Max Caps and Initials.
	- `"AmmoStandardInitial": 300 -> 168`
	- `"AmmoStandardInitialOnDropin": 200 -> 112`
	- `"AmmoStandardMaxCap": 690 -> 252`
	- `"AmmoSpecialInitial": 150 -> 84`
	- `"AmmoSpecialInitialOnDropin": 100 -> 56`
	- `"AmmoSpecialMaxCap": 345 -> 121`

	> `1.5` times ammo was too much for `2.0` times damage.

### 2.0.1

Fixed typos in README.

### 2.0.0

> a lot of new stuff!

#### Weapon balance:

> again, these changes may drastically change from previous experiense,
> to revert them, please delete `GameData_ArchetypeDataBlock_bin.json`

- Increased all weapon damage by `2.0` times

| NAME                 | CLASS               | DEFAULT DAMAGE | INCREASED |
|----------------------|---------------------|:--------------:|:---------:|
| Shelling S49         | Pistol              |           4.39 |      8.78 |
| Bataldo 3RB          | HEL Revolver        |           8.01 |     16.02 |
| Raptus Treffen 2     | Machine Pistol      |           1.81 |      3.62 |
| Raptus Steigro       | HEL Autopistol      |           1.01 |      2.02 |
| Accrat Golok DA      | Bullpup Rifle       |           1.91 |      3.82 |
| Van Auken LTC5       | SMG                 |           1.86 |      3.72 |
| Accrat STB           | PDW                 |           2.31 |      4.62 |
| Van Auken Cab F4     | Carbine             |           2.38 |      4.76 |
| Accrat ND6           | Heavy SMG           |           2.30 |      4.60 |
| TR22 Hanaway         | DMR                 |           7.51 |     15.02 |
| Malatack LX          | Assault Rifle       |           2.19 |      4.38 |
| Malatack CH 4        | Burst Rifle         |           2.71 |      5.42 |
| Drekker Pres Mod 556 | Rifle               |           5.08 |     10.16 |
| Hanaway PSB          | Double Tap Rifle    |           5.51 |     11.02 |
| Bataldo J 300        | HEL Shotgun         |          13.36 |     26.72 |
| Buckland SBS III     | Sawed-off Shotgun   |          30.40 |     60.80 |
| Malatack HXC         | Heavy Assault Rifle |           5.01 |     10.02 |
| Buckland S870        | Shotgun             |          30.10 |     60.20 |
| Buckland AF6         | Combat Shotgun      |          15.06 |     30.12 |
| Buckland XDIST2      | Choke Mod Shotgun   |          30.08 |     60.16 |
| Mastaba R66          | Revolver            |          14.21 |     28.42 |
| Techman Arbalist V   | Machinegun          |           5.35 |     10.70 |
| Techman Veruta XII   | Machinegun          |           3.51 |      7.02 |
| Techman Klust 6      | Burst Cannon        |          19.00 |     38.00 |
| Omneco Exp1          | HEL Gun             |          16.25 |     32.50 |
| High Caliber Pistol  | High Caliber Pistol |          25.10 |     50.20 |
| Precision Rifle      | Precision Rifle     |          11.40 |     22.80 |
| Köning PR 11         | Sniper              |          40.01 |     80.02 |
| Omneco LRG           | HEL Rifle           |          30.01 |     60.02 |

- Reduced hipfire spread on DMR.
	- `"HipFireSpread": 2.5 -> 1.0`

- Reduced reload time on Bullpup Rifle.
	- `"DefaultReloadTime": 2.4 -> 1.9`

- Giga-buffed the Sniper.
	- `"DefaultClipSize": 3 -> 6`
    - `"DefaultReloadTime": 3.5 -> 2.5`
	- `"PiercingBullets": false -> true`
	- `"HipFireSpread": 3.0 -> 0.5`

- Increased fire rate on HEL Rifle.
	- `"SpecialCooldownTime": 0.75 -> 0.12`

- Reduced recoil on High Caliber Pistol.
	- `"power":`
    	- `"Min": 12.0 -> 6.0`
    	- `"Max": 15.0 -> 7.0`

	> weapon balance is not fully tested,
	> more weapons would be tweaked
	> and some existing tweaks would be adjusted.

#### Flashlight adjustments:

- Increased angle for all other lights.
	- GunLight\_A `"angle": 65.0 -> 120.0`
	- GunLight\_B `"angle": 35.0 -> 100.0`
	- GunLight\_C `"angle": 40.0 -> 100.0`
	- GunLight\_E `"angle": 45.0 -> 120.0`

	> i realized that i hated not seeing shit.
	> distinctly remember `GunLight_B` being that of the 
	> sniper rifle.

#### Fog:

- Reduced infection buildup speed.
	- `"Infection": 0.03 -> 0.003`

	> fog annoying.

#### Melee Weapons:

- Buffed spear.
	- `"LightAttackDamage": 2.0 -> 3.0`
	- `"AllowRunningWhenCharging": false -> true`

	> literally everything other than hammer is considered bad,
	> so im looking into making other melee weapons good.

#### Player specs:

> these changes combined with weapon balance may not satisfy everyone,
> i will test them in a full team soon and may or may not revert them.
>
> until then i suggest you replace `GameData_PlayerDataBlock_bin.json`
> with one from previous release.

- Slightly increased movement speed.
	- `"walkMoveSpeed": 3.5, -> 4.08`
    - `"runMoveSpeed" 6.0, -> 7.0`
    - `"crouchMoveSpeed": 2.0, -> 2.33`

	> all multiplied by 7/6 because runMoveSpeed 7.0
	> felt good.

- Reduced all ammo caps to 1.5 times the default.
	- `"AmmoStandardMaxCap": 920 -> 690`
    - `"AmmoSpecialMaxCap": 460 -> 345`
    - `"AmmoClassMaxCap": 300 -> 225`

	> this is a setup for `GameData_ArchetypeDataBlock_bin.json` changes.

#### Upcoming:

> muh weapon balance tweaks coming :3

### 1.1.0 

#### Health changes:

- Effective max Health increased.
	- `"health": 50.0 -> 100.0`

- Increased Regeneration delay.
	- `"healthRegenStartDelayAfterDamage": 0.0 -> 3.0`

- Lowered Regen max value to `50%`.
	- `"healthRegenRelMax": 0.6 -> 0.5`

- Significantly increased Regen per second
	- `"healthRegenPerSecond": 0.5 -> 3.0`

	> testing out new settings that i wont die with,
	> but wont be too much of a bullet sponge either.
	>
	> also adding some fun nuance to packing.

#### Ammo tweaks:

- Increased Tool Ammo max cap
	- `"AmmoClassMaxCap": 150 -> 300`

	> idk it just didnt make sense ig.

#### Upcoming:

> next major version should include balance changes
> for all weapons, if it comes out!

### 1.0.1

- Updated "healthRegenPerSecond" to the correct value:
	- `1.0 -> 0.5`

### 1.0.0

- Release.