![Alt text](screenshot.png?raw=true "Paries snapshot")

# Paries
An automatic random background setter for LightDM GTK greeter.
# Why Paries?
Paries stands for 'wall' in Latin. I chose this name for the proximity relationship this word has with 'wallpaper', plain and simple.

It's been some time since I started to use LightDM GTK greeter in my computer, but I find the way it looks out of the box just boring. I have seen other OS login screens which displayed huge, high-res wallpapers that changed with time; and I thought I should implement this functionality in my own greeter.

# How does it work?
Do you really care about it? It's just magic.

Seriously, I have found that certain wallpaper provider website had its images classified by a unique numeric identificator. This represented an enormous advantage against bigger image hosting providers which just used the original name of the document for identifying their backgrounds. This way, I found it really easy to generate a wget instance that used the link to the website plus a random number to get a random wallpaper... ten times. The wallpapers, then, start changing in periods of two hours until the loop finsihes; time when it will start again during the next reboot.

# How to install
Make this script executable at startup, depending of your distribution. Also, modify your LightDM config file to select `lightdm-gtk-greeter` as your default greeter if you haven't done it already; as well as the greeter configuration file as well, replacing the default background path for `/usr/share/pixmaps/background.jpg` *(Psst... Uncomment the line or it won't work!)*

# WARNING:
Ah, I congratulate you for reading until here: some people will never know of the danger until it's too late for them. Listen up. 

It is really important for you to consider this is still a **proof-of-concept** program. I will add and improve more functionalities/documentation when I have time. Feel free to open an issue, fork and pull request this project if you think any aspect should be improved. Be careful: **an insane amount of NSFW content** (about 200.000 images which represent nearly 50% of the whole database) **has been detected.** 100% random wallpapers downloaded in packs of 10 contain at least one NSFW image. **I am working on fixing this issue as my main priority.** Nobody wants you to get fired, dumped or being forced to prepare a life-lesson themed speech to your children just for using your computer normally.

