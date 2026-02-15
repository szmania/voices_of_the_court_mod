# Frequently Asked Questions

## 1. No dialog box pops up
This mod requires an additional backend program to run. Download the localized backend program here: [https://github.com/szmania/Voices_of_the_Court/releases/latest](https://github.com/szmania/Voices_of_the_Court/releases/latest). The downloaded .exe file will install automatically upon opening.

## 2. API configuration issues
It is recommended to use the official DeepSeek API. In the dropdown menu for the dialogue model connection, select the `custom(openai-compatible)` page to configure:
- Server URL: `https://api.deepseek.com/beta`
- API Key: Enter your own API key, which can be applied for at [https://platform.deepseek.com](https://platform.deepseek.com).

OpenAI and OpenRouter should also be compatible.

## 3. No dialog box pops up even when the backend program is running after installation
**Solution**: You must use the localization mod.

Installation methods (choose one):
1. After extracting the downloaded localization mod files, overwrite the original mod files in the Steam Workshop directory directly.
2. Place the extracted mod folder `voices_of_the_court_mod-1.2.1-beta` into the game's mod folder. Then, use Notepad to create a new file named `voices_of_the_court_mod-1.2.1-beta.mod` in the `Documents\Paradox Interactive\Crusader Kings III\mod` folder with the following content:
version="1.0"
tags={
"Gameplay"
}
name="Voices of the Court mcc"
supported_version="1.13.1"
path="C:/Users/ [Your PC Username Here] / Documents/Paradox Interactive/Crusader Kings III/mod/voices_of_the_court_mod-1.2.1-beta"

If the dialog box still does not appear after installing and enabling the localization mod, the CK3 user folder path may be set incorrectly, or the game might be in Ironman mode. This mod does not work in Ironman mode.

## 4. Error "TypeError: Cannot read properties of undefined (reading 'playerID')" with red text when opening the chat window
**Solution**: Create a folder named `run` in `Documents\Paradox Interactive\Crusader Kings III`. Enter that folder and create a text file named `votc.txt`.

## 5. Recent memories are not being read when talking to characters
**Solution**:
1. This is a small bug in the original author's backend program; downloading the localized backend solves this.
2. It may also be due to memory token limits. Adjust the `max memory tokens` size in the backend program's settings page. After adjusting the memory tokens, you should also increase the `max new tokens`; it is best if `max new tokens` is larger than `max memory tokens`.

## 6. Prompt generation script reverts after restarting the backend program
**Solution**:
Save it as a separate file in the `custom` folder.


