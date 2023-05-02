# Dota Heroes Flutter Example UI

- [Resources](#resources)
- [Colors](#colors)
- [Home](#home)
- [Dota Hero Detail](#dota-hero-detail)

## Resources 

- Assets Images Download [Here](images)

## Colors

PrimarySwatch

- PrimaryBlack `#1E2328`

Content

- Primary `#FFFFFF`
- Secondary `#9B9B9B`
- Tertiary `#454545`

## Splash

<img src="readme_resources/splash.png"  width="240">

## Home

<img src="readme_resources/home.png"  width="240">

1. App Bar Bottom

    <img src="readme_resources/home_app_bar_bottom.png"  width="480">
    
    <img src="readme_resources/home_app_bar_bottom_padding.png"  width="480">
    
    - Filter Primary Attribute (Deselected Opacity `0.25`)
    - Sort
      - Ascending Icon `CupertinoIcons.sort_down`
      - Descending Icon `CupertinoIcons.sort_up`
    - Show Favorite Icon `CupertinoIcons.heart_fill` (Deselected Opacity `0.25`)
    - SearchBar PrefixIcon `CupertinoIcons.search`
      
2. Grid
    
    <img src="readme_resources/home_grid.png"  width="480">
    
    <img src="readme_resources/home_grid_padding.png"  width="480">
    
3. Tile
    
    <img src="readme_resources/home_tile.png"  width="300"> <img src="readme_resources/home_tile_padding.png"  width="300">

    - AspectRatio `16.0 / 9.0`
    - Shadow `Colors.black54` with `Offset(0,2)`
    - Show Favorite Icon `CupertinoIcons.heart_fill` with **Content Primary Color** if already added to favorites
    - Name Container gradient from **Top** `Colors.transparent` to **Bottom** `Colors.black87`
      
## Dota Hero Detail

<img src="readme_resources/dota_hero_detail.png"  width="240">

1. Header

    <img src="readme_resources/dota_hero_detail_header.png"  width="480">
    
    <img src="readme_resources/dota_hero_detail_header_padding.png"  width="480">

    - Example potrait image url `https://cdn.cloudflare.steamstatic.com/apps/dota2/videos/dota_react/heroes/renders/crystal_maiden.png`
    
2. Attributes

    <img src="readme_resources/dota_hero_detail_attributes.png"  width="480">
    
    <img src="readme_resources/dota_hero_detail_attributes_padding.png"  width="480">
    
    - Grident background from **Left** `#252728` to **Right** `#101415`
    - Health Bar Grident background from **Left** `#286323` to **Right** `#7AF03C`
    - Mana Bar Grident background from **Left** `#1056DB` to **Right** `#73F5FE`
    - Health = `baseHealth` + (`baseStr` * 20.0)
    - HealthRegen = `baseHealthRegen` + (`baseStr` * 0.1)
    - Mana = `baseMana` + (`baseInt` * 12.0)
    - ManaRegen = `baseManaRegen` + (`baseInt` * 0.05)
    
3. Roles

    <img src="readme_resources/dota_hero_detail_roles.png"  width="480">
    
    <img src="readme_resources/dota_hero_detail_roles_padding.png"  width="480">
    
    - Grident background from **Left** `#252728` to **Right** `#101415`
    
4. Stats

    <img src="readme_resources/dota_hero_detail_stats.png"  width="480">
    
    <img src="readme_resources/dota_hero_detail_stats_padding.png"  width="480">
    
    - Grident background from **Left** `#252728` to **Right** `#101415`
    - AttackMin if Primary Attribute
      - Strength: `baseAttackMin` + `baseStr`
      - Agility: `baseAttackMin` + `baseAgi`
      - Intelligence: `baseAttackMin` + `baseInt`
      - Universal: `baseAttackMin` + (`baseStr` * 0.6) + (`baseAgi` * 0.6) + (`baseInt` * 0.6)
    - AttackMax if Primary Attribute
      - Strength: `baseAttackMax` + `baseStr`
      - Agility: `baseAttackMax` + `baseAgi`
      - Intelligence: `baseAttackMax` + `baseInt`
      - Universal: `baseAttackMax` + (`baseStr` * 0.6) + (`baseAgi` * 0.6) + (`baseInt` * 0.6)
    - Armor = `baseArmor` + (`baseAgi` * 0.167)
   
