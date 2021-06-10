
<img src = "https://github.com/ChanJianHao/SubMe/blob/master/resources/SubMe.png?raw=true"><br>
# SubMe 

A cloud deployment of [Autosub](https://github.com/BingLingGroup/autosub) on Google Colab. It leverages Google's cloud computing clusters and GPU to automatically generate subtitles for uploaded video files in various languages. Audio is first pre-processed using `ffmpeg` and `ffmpeg-normalize`. Speech recognition is then conducted on the pre-processed audio using `Auditok`, after which `ffmpeg` will be used to splice the audio files into individual segments. The segments will be transcribed using Google's Cloud Speech-to-Text API, then translated into your desired language using `py-googletrans`. 


## Why use our tool? 
Firstly, its free! Other similar products, such as [Veed](https://www.veed.io/pricing), are paid services with restrictions on video length. We offer a completely free service with no restrictions on video length. 

Secondly, our tool significantly speeds up the runtime of Autosub. A [study](https://towardsdatascience.com/google-colab-how-does-it-compare-to-a-gpu-enabled-laptop-851c1e0a2ca9) has shown that despite being a free service, the GPU-enabled Google Colab environment (which is what we are using now) is significantly faster than a GPU-enabled MacBook Pro, Lenovo Legion and Lenovo Thinkpad, contributing to greater time savings. 

Thirdly, without the need to provision and maintain expensive hardware, users will also enjoy greater cost savings. Moreover, you will no longer have to worry about overheated machines or exorbitant electricity bills. 

Fourthly, we have an easy to use interface. No need to concern yourself with the complex technology of voice extraction and language translation. Just click and few buttons and you’re set. 

Lastly, our tool will also help the less fortunate, such as those with hearing disabilities, to decipher what is being spoken in videos and movies. 
## Getting Started
- Click on <a href="https://colab.research.google.com/github/ChanJianHao/SubMe/blob/master/SubMe.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> to open the notebook in Google Colab. <br>
- Follow the instructions on the notebook
### Uploading from Google Drive

<img src="https://i.imgur.com/ragE2y4.png" width="75%" height="75%">
When you encounter the above screen, click on the link and a new tab will be opened. 

<img src="https://i.imgur.com/Z3LsX8M.png" width="25%" height="25%">
Click allow. A code will be generated. Copy the code and paste it into the empty field in the notebook. Press Enter.

<img src = "https://github.com/ChanJianHao/SubMe/blob/master/resources/File.png?raw=true" width="25%" height="25%">
After successfully mounting Google Drive, you will be able to access your directory by clicking on File on the left.


### Output

When uploading, you will have to specify the extension of the output files (`srt`, `ass`, `sub`, `json` or `txt`). The output files can be found in the same directory as the uploaded video file. For example, if you uploaded a video file from `/content/drive/My Drive`, the subtitle file will also be found here.

When downloading, the output files can be found in `/content/drive/My Drive/Torrent`.

### Updates

10 June 2021 - Subtitling/captioning of video is now possible. Just put the same language code for source and destination language and autosubs will generate subtitles for your video in its original language.

## Authors
We are two Singaporean university undergraduates with curiosity and passion for social causes. In particular, we are interested in using technology to benefit the less fortunate people in our society.

* [**Chan Jian Hao**](https://github.com/ChanJianHao)
* [**Ng Wei Jie**](https://github.com/HandsomeWJ)

## Acknowledgments
* [agermanidis](https://github.com/agermanidis/autosub)
* [BingLingGroup](https://github.com/BingLingGroup)



