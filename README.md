# Pain Silhouette

**[English](#english) · [Русский](#русский)**

## English

A small HUD for *Casualties: Unknown* that shows **where it hurts, not what the injury is**. If your character's left leg starts shaking, you know that's where they feel pain. The silhouette won't tell you whether the leg is broken, dislocated, or bleeding. For a closer look, open the health menu as usual.

### Reading the silhouette

The silhouette uses the body diagram from the game's health menu. **Movement shows pain; colour follows the game's own damage display.** On an ordinary limb, the outline represents skin condition and the fill represents muscle condition. If you play without a chip, the fill follows the game's unchipped display instead. There are no injury labels, percentages, or treatment buttons. The mod changes the display, not the way pain, damage, or healing works.

### Installation

1. Install [BepInEx 5.4.x](https://github.com/BepInEx/BepInEx/releases) for **Unity Mono** in the game folder, unless it's already installed. Run the game once and quit so BepInEx creates its folders.
2. Open **Releases**, select the latest version, and download **`PainSilhouette.dll`** under **Assets**. Put the DLL in the game's `BepInEx/plugins/` folder.
3. Launch the game. Press **F6** during play to hide or show the silhouette. You can change that key in the settings.

The same DLL is intended for the full game and the Steam demo. Install it in the folder of the version you play. The HUD shows your own character. I haven't tested it with another player in *Casualties Together* yet.

### Settings

You can move and resize the silhouette, change its opacity, or turn off the brief flash when a limb takes damage. **Pain shake** makes the movement easier to see on a small HUD: **×1** matches the health menu, **×2** is the default, and the slider goes up to **×5**. It does **not** make the character feel more pain. By default the HUD hides during sleep and minigames, but stays visible while crafting. Each has its own setting.

The mod saves its settings **only** in `BepInEx/config/evzaharof.painsilhouette.cfg`. Close the in-game Settings menu to save your changes. You can also edit the file for precise values beyond the sliders. For example, `Size = 0.4` means 40%. To reset **only this mod**, quit the game and delete that `.cfg`. The next launch recreates it with the defaults. Leave the game's `settings.json` alone.

### A note from me

I'm a little embarrassed to admit it, but AI wrote most of the code for this mod. I don't know C# very well, and I was more interested in making the mod than in learning the language.

### Contact

You can message me on Telegram at [@evzaharof](https://t.me/evzaharof) with any questions. Bug reports and ideas are welcome too. If possible, please write in Russian - I don't speak English.

---

## Русский

Мод для *Casualties: Unknown*, который показывает, **где болит, а не чем именно травмирован персонаж**. Если у силуэта дрожит левая нога, значит, персонаж чувствует там боль. Сломана ли нога, есть ли вывих или кровотечение - силуэт не подскажет. Для осмотра по-прежнему нужно открыть меню здоровья.

### Как читать силуэт

Это уменьшенная копия куклы из меню здоровья. **Дрожь показывает боль, а цвет повторяет подсветку повреждений из игры.** У обычной конечности контур показывает состояние кожи, а заливка - мышц. Если персонаж без чипа, заливка меняется по тем же правилам, что и в игре без чипа. На силуэте нет названий травм, процентов или кнопок лечения. Мод не меняет боль, урон или лечение - только то, что видно на экране.

### Установка

1. Если [BepInEx 5.4.x](https://github.com/BepInEx/BepInEx/releases) для **Unity Mono** ещё не установлен, установи его в папку игры. Один раз запусти игру и выйди, чтобы BepInEx создал свои папки.
2. Открой **Releases**, выбери последнюю версию и скачай **`PainSilhouette.dll`** из раздела **Assets**. Положи DLL в папку `BepInEx/plugins/` внутри папки игры.
3. Запусти игру. Во время игры **F6** скрывает и показывает силуэт. Клавишу можно поменять в настройках.

Одна DLL рассчитана на полную игру и демоверсию Steam. Устанавливай её в папку той версии, в которую играешь. Кукла показывает твоего персонажа. С другим игроком в *Casualties Together* я мод пока не проверял.

### Настройки

Силуэт можно передвинуть, изменить его размер и прозрачность или отключить короткую вспышку при получении урона. **Pain shake** помогает заметить дрожь на маленькой кукле: **×1** - как в меню здоровья, **×2** - по умолчанию, **×5** - максимум ползунка. Усиливается **только дрожь на экране**, а не боль персонажа. По умолчанию кукла скрывается во сне и в мини-играх, но остаётся видна при крафте. Для каждого случая есть отдельная галочка.

Настройки мода хранятся **только** в `BepInEx/config/evzaharof.painsilhouette.cfg`. Чтобы сохранить изменения из вкладки, закрой меню настроек. В самом файле можно вписать точные значения, в том числе за пределами ползунков: например, `Size = 0.4` означает 40%. Чтобы сбросить **только мод**, закрой игру и удали этот `.cfg`. При следующем запуске он появится заново со стандартными значениями. Удалять игровой `settings.json` не нужно.

### От автора

Немного неловко признаваться, но большую часть кода для мода написал ИИ. Я в C# не особо разбираюсь, а сделать мод хотелось больше, чем учить язык.

### Связь со мной

Пиши мне в Telegram: [@evzaharof](https://t.me/evzaharof). Можно обращаться по любым вопросам. Если найдёшь баг или захочешь предложить идею, тоже пиши. Я говорю по-русски, так что переводить сообщение на английский не нужно.
