# Better Weapon Durability

BetterWeaponDurability gives you full control over weapon durability and battery drain stuff. You can modify the drain rates for melee weapons and guns (not drones or orbs though, they suck to deal with, I have no idea what value does what for orbs and drones)

- **Melee:** Adjusts `durabilityDrain` and `durabilityDrainOnEnemiesAndPVP` by an additive offset. Lower (negative) offsets reduce drain, making weapons more durable.
- **Guns:** Adjusts the guns `batteryDrain` by an additive offset. Lower offsets reduce drain per shot

## Installation

1. **Using r2modman (Recommended):**
   - Download the latest version from Thunderstore.
   - Open r2modman and select your R.E.P.O. profile.
   - Click on the Get Mods button to the left and find this mod and download it.
   - Enable the mod and launch the game.

2. **Manual Installation:**
   - Extract the contents of the mod package.
   - Copy the `BetterWeaponDurability.dll` file or the `FancyDucc-BetterWeaponDurability` folder into your `BepInEx/plugins/` folder.
   - Make sure that the mod’s folder has the `manifest.json` and `icon.png` if you want it to appear in r2modman as a local package.

## Configuration

### This mod does nothing without changing the values, you need to change the config to see anything happen.

This mod has support and stuff for RepoConfig, use that, it's good for this.

### ItemMelee Settings
- **DrainOffset:**  
  *Type:* Float  
  *Range:* -500 to 100  
  *Default:* 0.0

### ItemGun Settings
- **BatteryDrainOffset:**  
  *Type:* Float  
  *Range:* -100 to 500  
  *Default:* 0.0  

  **Note:** The mod forces `batteryDrainFullBar` to false so the offset takes effect, I don't know if this breaks something, but in testing, nothing with weapons seemed to be weird.

## Usage

1. **Launch R.E.P.O.** using r2modman with BetterWeaponDurability enabled.
2. **Open REPOConfig** if you have it installed.
3. Find**BetterWeaponDurability** in the mod list and adjust the settings.
4. Changes are applied live but only on the main menu, so if you want to change your settings, you'll have to go back to the main menu to change them, but no relaunching the game is needed :D

## Dependencies

- **BepInEx** – mmmm, bepinex... yeah, this is needed for literally any mod to work for R.E.P.O. If you don't have this, you don't have mods.
- **REPOConfig** – Let's you configure mod stuff in-game. This isn't really a dependency, it works without it, but it's nice to have.