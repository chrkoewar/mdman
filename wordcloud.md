# wordcloud

generate a world cloud image file from data file; also by image mask

## cmd
```
word_cloud ... tikz/svg https://github.com/amueller/word_cloud/issues/493
prepare tag data for wordcloud
launch via wordcloud_cli or with python scripts
rg -oP '[¬·]\w+' *.txt | sed 's/^[^:]*://' | awk '{print tolower($0)}' | cut -c 2- | shuf
pip install wordcloud
wordcloud_cli --text shuffled.txt --imagefile ttt.png --mask stormtrooper_mask.png --width 800 --height 600
wordcloud_cli --text test --imagefile frequency.png --max_words N
https://github.com/amueller/word_cloud
CLI     wordloud_cli
```
