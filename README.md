[Tiếng Việt](README_VN.md)
# Why fcitx-unikey?
Many of you have probably knew ibus-unikey or ibus-bamboo as Vietnamese typing tool in Linux. However, using ibus-unikey or ibus-bamboo with the latest WPS Office for Linux (wps-2019-snap on SNAP, build 9125) causes significant slowdown when starting up WPS office software. (Note: don't use the current official deb package from wps office site, as they don't even show Vietnamese typing at all, for both ibus and fcitx). I find that fcitx-unikey does not cause such slowdown, which is possibly due to some kind of qt-gtk incompatibility of ibus modules. Beside, instructions of how to set up fcitx-unikey are scattered and incomplete. Therefore, I decide to write this guide as a comprehensive, step-by-step instruction with screenshots to help you set up fcitx-unikey easier.

# Step-by-step Instruction
1. First, you need to install Vietnamese Language. Make sure you're online. Go to Start --> Settings --> Language Support

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/1.%20Settings%20Language.png)

2. If there are any warning about incomplete language package, ignore it. Then hit the "Install/Remove Languages..." button:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/2.%20Install%20New%20Language.png)

3. Scroll down and double click on "Vietnamese" to make it bold, and the text "1 to install" appear:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/3.%20Install%20Vietnamese.png)

Then hit "Apply". This will start downloading all the required modules for Vietnamese, including - fortunately - fcitx and fcitx-unikey! After it's done, log out and log back in (or perform a reboot).

4. Open the Language Support dialog again (Start --> Settings --> Language Support). This time, change "Keyboard Input Method System" to "fcitx":

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/4.%20Change%20Input%20Method.png)

5. Now, start fcitx service by going to Start --> System --> Fcitx:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/5.%20Start%20fcitx.png)

6. An icon in the status notification bar with an "a" appear. Left click on it and then click "Configure":

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/6.%20Configure%20fcitx.png)

7. We need to add Unikey as a new Input Method. To do so, click on the Plus "+" icon near the lower left corner of the fcitx configure dialog:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/7.%20Add%20New%20Input%20Method.png)

8. Untick "Only Show Current Language", then type "Unikey" in the search box (case sensitive, make sure it's the big "U"), and choose Unikey, then hit OK:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/8.%20Unikey.png)

9. You should have two input methods at this step:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/9.%20Final%20Input%20Methods.png)

10. In "Global Config" tab, you can change the "Trigger Input Method" hot key to a different key combination. Mine is Alt+Z to make it similar to Unikey in Windows:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/10.%20Switch%20Keyboard%20Shortcut.png)

11. Under "Appearance" tab, increase the font size of the "hint" box that appear when you're typing Vietnamese in WPS Office (see the last picture, step 13):

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/11.%20Hint%20Appearance.png)

12. To switch input methods (i.e. between English and Vietnamese typing), you can use the hot key defined in step 10, or left click on the fcitx icon in the status notification bar --> Input Method. Note that fcitx input method only changes when your mouse is pointing to an editable field. It won't change if, says, you're on desktop and not typing.

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/12.%20Switch%20Input%20Method.png)

13. Here is the "hint" box and how it looks like in WPS Office Writer:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/13.%20WPS%20Unikey%20Demo.png)
