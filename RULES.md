# Rules for Publishing and Updating Plugins in the Repository

These rules are aimed not only at security but also at the benefit and convenience of the user.

## 1. Metadata
1.1 A plugin must include `__id__`, `__name__`, `__author__`, `__version__`, and `__description__`.  
1.2 The plugin ID must be unique and not duplicate any other plugin's ID.  
1.3 A plugin icon is optional, but if provided, it should not be a random sticker—it should genuinely relate to or reflect the plugin's subject matter.  
1.4 The version must contain the plugin version number without the "v" prefix at the beginning of the version string.  
1.5 The plugin description must not overstate its functionality or falsely imply that it can do more than it actually can.

## 2. Functionality
2.1 The plugin must not be just for laughs, as a joke, purely for entertainment, or otherwise useless.  
2.2 The plugin must not be malicious or exhibit suspicious behavior.  
2.3 The plugin must not duplicate an existing one, except in cases where it is superior to the existing plugin.  
2.4 The plugin must not add badges to its own developers.  
2.5 The plugin must not have mandatory auto-updates.  
2.6 The plugin must not include functionality unrelated to its core theme *(e.g., making a voice-changer plugin and bundling your own badge system into it)*.  
2.7 The plugin must not contain screamers or unpleasant Easter eggs.  
2.8 The plugin must not collect user data or statistics.  
2.9 The plugin must not display unnecessary notifications, bulletins, or dialogs upon client startup or during use unless they are actually needed.  
2.10 The plugin must not contain advertising or paid features.

## 3. Quality
3.1 If a plugin supports multiple languages, it must automatically choose the user's language as set in the client (not the system) *(e.g., the client language can be detected via `java.util.Locale`)*.  
3.2 If the plugin contains labels, text, notifications, or text processing, they must at minimum support English or Russian, except for plugins specifically targeting an audience from a particular country/countries where the language(s) used in the plugin are official state languages.  
3.3 The plugin must not overload the client or cause lag.  
3.4 Plugin settings must be placed in the settings menu (`create_settings`), not via chat commands.  
3.5 Plugin settings must have a `link_alias` to provide users with convenient links to specific settings.  
3.6 The plugin must actually perform its advertised functionality.  
3.7 The plugin must not be excessively unstable or have critical bugs that hinder its use.  
3.8 Features that would be more conveniently accessed via a menu button must be implemented as a menu button, not solely as a chat command.  
3.9 The plugin must properly clean up its data, hooks, etc., upon deactivation (`on_plugin_unload`) so that no traces or side effects remain.  
3.10 The plugin must not annoy or inconvenience the user.

## 4. Moderation
4.1 If the plugin contains compiled or obfuscated parts, their source code, build instructions, and configurations must be provided for self-compilation.  
4.2 Do not spam with messages, plugin proposals, or resubmissions of already rejected plugins.  
4.3 The rules may change over time, or I may simply dislike the quality, functionality, or purpose of a plugin. Therefore, some plugins may be rejected or removed even if they do not formally violate any of the above rules.