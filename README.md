# ConverterPreset4foobar2000
fb2k 自用转换器模版

* FLAC L8 Album [Hi] [Discs] to
```
%album artist% - [%date% - ]%album%$if($or($greater(%__bitspersample%,16),$greater(%samplerate%,44100)), - %__bitspersample%Bit%samplerate%Hz)/[Disc$num(%discnumber%,2)/][$num(%discnumber%,2)-]$num(%tracknumber%,3) - [%artist% - ]%title%
```

* FLAC L8 Artist Album [Hi] [Discs] to
```
%album artist%/%album artist% - [%date% - ]%album%$if($or($greater(%__bitspersample%,16),$greater(%samplerate%,44100)), - %__bitspersample%Bit%samplerate%Hz)/[Disc$num(%discnumber%,2)/][$num(%discnumber%,2)-]$num(%tracknumber%,3) - [%artist% - ]%title%
```

* AAC 320K For iPod
```
$num(%discnumber%,2)-$num(%tracknumber%,3) - $if2(%artist%,Unknown Artist) - %title%
```

* ALAC For PC
```
$num(%discnumber%,2)-$num(%tracknumber%,3) - $if2(%artist%,Unknown Artist) - %title%
```
