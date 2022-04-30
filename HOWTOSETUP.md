# 설정 방법

### Animation

Figma Prototype을 녹화 한 후 파일로 저장

### Mov -> Gif

https://github.com/vvo/gifify 을 통해 동영상을 Gif로 변환

명령어

`gifify input_vedio.mov -o output.gif --fps 60 --no-loop`

### Gif -> Svg로 변환

https://github.com/tomkwok/svgasm 을 통해 Gif를 Svg로 변환

명령어 (흑백 기준)

`svgasm -t 'mkbitmap -x -t 0.44 -s 1 "%s" -o - | potrace --svg -o -' -s 'svg {background-color: white}' -d 1/60 -i 1 -l '' input.gif > output.svg`
