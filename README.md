<div align="center">

# Tweak Click (Port / Fork)

**Language / Язык:**  
[🇬🇧 English](#english) • [🇷🇺 Русский](#russian)  
<sub>*(Standalone files: [English](README_EN.md) | [Русский](README_RU.md))*</sub>

</div>

---

<span id="english"></span>
## 🇬🇧 English

> [!IMPORTANT]
> **Disclaimer:**
> This repository is an **unofficial fork** of the Tweak Click mod.
> 
> * **Original Author:** [shane04111](https://github.com/shane04111)
> * **Original Repository:** [shane04111/Tweak-Click](https://github.com/shane04111/Tweak-Click)
> * **Modrinth Page:** [modrinth.com/mod/tweak-click](https://modrinth.com/mod/tweak-click)
> * **Original License:** MIT
> 
> This fork was created solely to port and adapt the mod for **Minecraft 26.3**, migrating to the unobfuscated `Identifier` API, updating Loom to 1.18+, adjusting screen handling to `mc.gui.screen()`, and updating dependencies for Java 25. All rights to the original code, concept, and assets belong to the original author.

### 🌟 About
**Tweak Click** is a client-side technical Minecraft mod and extension for [Tweakeroo](https://github.com/sakura-ryoko/tweakeroo) (built on Fabric and [MaLiLib](https://github.com/sakura-ryoko/malilib)). It provides quality-of-life tweaks for technical players, tunnel digging, and perimeter construction:

* **onlySprintHoldAttack (Hold Attack While Sprinting):** Automatically holds down the attack/mine key (LMB) only while sprinting when Tweakeroo's `tweakToolSwitch` is enabled. Stops attacking when walking or standing still.
* **movementWillHold:** Allows holding the attack key while walking too (not only sprinting).
* **flatDigger (Flat Digging):** Prevents accidentally breaking blocks under your feet while running/mining forward, ensuring a flat floor. Sneak (Shift) to dig blocks below you.
* **verticalDigger (Vertical Digging):** Restricts mining strictly to vertical blocks (directly above or below) while sneaking, preventing accidental side breaks in 1x1 shafts.
* **diggerX / diggerZ (Axis Digging):** Only allows digging blocks along the specified coordinate axis (X or Z) when not sneaking, ideal for carving straight trenches.
* **removeCooldown (Remove Breaking Cooldown):** Removes the vanilla 5-gametick (0.25s) delay after breaking a block before mining the next one.
* **useItemDoNotEat:** Prevents accidentally eating carrots and potatoes when spamming right-click to plant them.
* **perimeterWallDigger:** Prevents mining underneath block types specified in the `perimeterOutlineBlocks` list for perimeter trenches and quarry layouts.

### ⌨️ Controls
* **Open Settings Menu:** Hold **`X`** and press **`C`** by default (Tweakeroo menu).
* Tweak Click's options appear directly at the top of Tweakeroo's **Tweak Toggles** / **Generic** lists.
* Settings are also accessible via **Mod Menu** (gear icon next to Tweakeroo).

### 📦 Dependencies
* [Fabric Loader](https://fabricmc.net/) (>= 0.19.0)
* [Fabric API](https://curseforge.com/minecraft/mc-mods/fabric-api)
* [MaLiLib](https://github.com/sakura-ryoko/malilib) (>= 0.30.0)
* [Tweakeroo](https://github.com/sakura-ryoko/tweakeroo) (>= 0.30.0)

### 🛠️ Building from Source
This project uses the Fallen-Breath preprocessor to build for targeted versions. Requires **JDK 25**.

Build version 26.3:
```bash
./gradlew :26.3:build
```
The compiled JAR file will appear in `versions/26.3/build/libs/tweakclick-mc26.3-v0.5.0.jar`.

---

<span id="russian"></span>
## 🇷🇺 Русский

> [!IMPORTANT]
> **Отказ от авторства:**
> Этот репозиторий является **неофициальным форком** мода Tweak Click.
> 
> * **Оригинальный автор:** [shane04111](https://github.com/shane04111)
> * **Оригинальный репозиторий:** [shane04111/Tweak-Click](https://github.com/shane04111/Tweak-Click)
> * **Страница на Modrinth:** [modrinth.com/mod/tweak-click](https://modrinth.com/mod/tweak-click)
> * **Лицензия оригинала:** MIT
> 
> Этот форк создан исключительно с целью портирования и адаптации мода под **Minecraft 26.3**, перехода на деобфусцированный API `Identifier`, адаптации экрана под `mc.gui.screen()`, обновления Loom до версии 1.18+ и поддержки Java 25. Все права на оригинальный код, идею и графику принадлежат оригинальному автору.

### 🌟 О моде
**Tweak Click** — это клиентский технический мод для Minecraft и аддон к [Tweakeroo](https://github.com/sakura-ryoko/tweakeroo) (на базе Fabric и [MaLiLib](https://github.com/sakura-ryoko/malilib)). Он добавляет полезные твики для технических игроков, копания туннелей и обустройства периметров:

* **onlySprintHoldAttack (Авто-атака при спринте):** автоматически зажимает ЛКМ (копание/атака), только пока вы бежите на спринте при включённом `tweakToolSwitch` в Tweakeroo. При остановке или переходе на шаг атака сразу прекращается.
* **movementWillHold:** зажимает кнопку атаки при любом движении (включая обычную ходьбу, а не только спринт).
* **flatDigger (Ровный пол):** защищает от случайного выкапывания блоков под ногами при беге/копании вперёд. Чтобы сломать блок под собой, нужно зажать Shift.
* **verticalDigger (Вертикальное копание):** при зажатом Shift разрешает копать блоки только строго вертикально вверх или вниз (шахта 1x1), блокируя случайные клики по боковым стенам.
* **diggerX / diggerZ (Копание по осям):** ограничивает копание блоков строго по координатной оси X или Z при обычном движении, идеально для прямых траншей и туннелей.
* **removeCooldown (Удаление задержки копания):** убирает ванильную задержку в 5 тиков (0.25 сек) перед началом разрушения следующего блока.
* **useItemDoNotEat:** предотвращает случайное съедание моркови или картофеля, когда вы зажимаете ПКМ при их посадке на грядки.
* **perimeterWallDigger:** запрещает копать блоки под типами блоков, указанными в списке контура `perimeterOutlineBlocks` (для разметки периметров).

### ⌨️ Управление
* **Открыть меню настроек:** по умолчанию зажать **`X`** и нажать **`C`** (меню Tweakeroo).
* Опции Tweak Click встраиваются прямо в начало списка **Tweak Toggles** / **Generic** мода Tweakeroo.
* Также настройки доступны через **Mod Menu** (шестерёнка напротив Tweakeroo).

### 📦 Зависимости
* [Fabric Loader](https://fabricmc.net/) (>= 0.19.0)
* [Fabric API](https://curseforge.com/minecraft/mc-mods/fabric-api)
* [MaLiLib](https://github.com/sakura-ryoko/malilib) (>= 0.30.0)
* [Tweakeroo](https://github.com/sakura-ryoko/tweakeroo) (>= 0.30.0)

### 🛠️ Сборка из исходников
Проект использует препроцессор Fallen-Breath. Для сборки требуется **JDK 25**.

Сборка версии 26.3:
```bash
./gradlew :26.3:build
```
Собранный JAR-файл появится в папке `versions/26.3/build/libs/tweakclick-mc26.3-v0.5.0.jar`.
