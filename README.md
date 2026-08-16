# Extera Plugins
exteraGram Plugin Catalog

```
tg://packit?repo=add&name=Crystal&link=https://github.com/AlexeiCrystal/extera-plugins/raw/main/packit/repomap.json
```

Wan't to add/update plugin? See [publishing rules](RULES.md)

# Repository structure
- **The [plugins](plugins/) folder contains plugin files**
- **The [packit](packit/) folder contains:**
    - [repomap.json](packit/repomap.json) – the main repository configuration for PackIt
    - [plugins.json](packit/plugins.json) – the list of plugins for PackIt
    - [process_new_plugin.py](packit/process_new_plugin.py) – a script for automatically updating [plugins.json](packit/plugins.json) when a plugin file is added, modified or removed from the [plugins](plugins/) folder; it runs automatically via a workflow